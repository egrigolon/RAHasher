# CLI macOS/Linux Port Plan

Goal: port only the `RAHasher` CLI so macOS and Linux can validate local game hashes against RetroAchievements hashing rules. The GUI/libretro app is out of scope.

## Scope boundaries

- In scope: `Makefile.RAHasher`, `Makefile.common`, CLI code reachable from `src/RAHasher.cpp`, `src/Hash3DS.cpp`, `src/HashCHD.cpp`, `src/Util.cpp`, and bundled hashing deps.
- Out of scope: root `Makefile`, `RALibretro.exe`, SDL UI, `Application.cpp`, updater/download flow, WinHTTP, libretro core loading, Visual Studio GUI targets.
- Preserve current CLI behavior documented in `AGENTS.md`, especially `?` auto-detect and multi-file/glob rules.

## Suggested branches

- `port/cli-posix-build` for Makefile/platform cleanup and non-CHD builds.
- `port/cli-chd-support` only if CHD work grows beyond small follow-up fixes.

## Work packages

### 1. Baseline and reproducibility

- [ ] Capture current build behavior on the target machine: OS, architecture, compiler, and failing command output.
- [ ] Try non-CHD CLI build first: `make -f Makefile.RAHasher`.
- [ ] Try CHD CLI build separately: `make clean && make -f Makefile.RAHasher HAVE_CHD=1`.
- [ ] Record whether output lands in `bin/` or `bin64/` and whether that matches `ARCH`.

### 2. Makefile portability

- [ ] Keep CLI build isolated to `Makefile.RAHasher`; do not make the root GUI `Makefile` portable unless strictly required.
- [ ] Adjust `Makefile.common` so macOS/Linux do not receive unsupported flags such as `-static-libgcc`, `-static-libstdc++`, or inappropriate `-m32/-m64` values.
- [ ] Prefer explicit `ARCH=x64` / `ARCH=arm64` handling over guessing when compiler support differs by OS.
- [ ] Ensure generated `src/RA_BuildVer.h` still works from `.git/HEAD`.
- [ ] Keep `HAVE_CHD=1` optional and make non-CHD builds useful.

### 3. CLI source portability

- [ ] Audit only code compiled with `_CONSOLE`; avoid fixing GUI-only Windows code.
- [ ] Verify Unix paths in `src/RAHasher.cpp` still rely on shell glob expansion and POSIX filesystem APIs.
- [ ] Check `src/Util.cpp` for functions included in `_CONSOLE` builds and guard or replace any accidental Windows-only calls.
- [ ] Preserve zip, 3DS, disc, and normal ROM hashing paths.
- [ ] Keep CLI output format stable so scripts can compare hashes.

### 4. CHD support

- [ ] Build with `HAVE_CHD=1` after the non-CHD CLI succeeds.
- [ ] Fix only bundled `libchdr`/lzma/zlib/zstd compile or link issues needed by CLI.
- [ ] Verify CHD support fails clearly when `HAVE_CHD` is omitted and works when included.

### 5. Verification

- [ ] Run the smallest relevant successful build after each package.
- [ ] Run `RAHasher` without args and confirm usage/console list prints.
- [ ] Verify a known ROM hash against an expected RetroAchievements hash.
- [ ] Verify `?` auto-detect on a single file.
- [ ] Verify multi-file mode rejects or avoids `?` auto-detect as before.
- [ ] If CHD is enabled, verify one known CHD hash.

## Expected effort

- Linux CLI: low effort, mostly build cleanup and verification.
- macOS CLI: low-to-medium effort; Apple Silicon may need extra architecture flag cleanup.
- CHD support is the most likely source of extra work.

## Completion criteria

- [ ] `make -f Makefile.RAHasher` succeeds on macOS or Linux.
- [ ] `make clean && make -f Makefile.RAHasher HAVE_CHD=1` succeeds or CHD limitations are documented.
- [ ] CLI behavior matches existing documented behavior for single-file, multi-file, glob, and `?` cases.
- [ ] No GUI/libretro porting work was introduced accidentally.
