# AGENTS.md

## Repo shape
- This repo builds two programs from the same `src/` tree: CLI hasher `src/RAHasher.cpp` and GUI/libretro app `src/main.cpp`/`src/Application.cpp`.
- `Makefile.RAHasher` builds the CLI (`RAHasher`); root `Makefile` builds the GUI/libretro app (`RALibretro.exe`). Do not assume `make` builds the CLI.
- Important submodules live under `src/SDL2`, `src/jsonsax`, `src/miniz`, `src/RAInterface`, `src/rcheevos`, and `src/libchdr`; clone/update with submodules when dependencies are missing.

## Build and verification commands
- CLI release with CHD support: `make -f Makefile.RAHasher HAVE_CHD=1`.
- CLI debug: `make clean && make -f Makefile.RAHasher HAVE_CHD=1 DEBUG=1`.
- GUI/libretro release: `make`; GUI debug: `make clean && make DEBUG=1`.
- Force architecture when needed: `ARCH=x86` writes to `bin/`, `ARCH=x64` writes to `bin64/`.
- Linux CI mirrors: `make ARCH=x86 HAVE_CHD=1 -f Makefile.RAHasher` and `make ARCH=x64 HAVE_CHD=1 -f Makefile.RAHasher`.
- Windows CI builds the CLI with `msbuild.exe RALibretro.sln -t:RAHasher -p:Configuration=Release -p:Platform=x86|x64`.
- No test, lint, or typecheck target is present; use the smallest relevant build as verification.

## Build quirks
- Run `make clean` before switching release/debug; object files are shared and flags differ.
- `src/RA_BuildVer.h` is generated during builds from `.git/HEAD`; it is ignored and should not be committed.
- CHD hashing is compiled only when `HAVE_CHD=1`; without it, CHD inputs report unsupported behavior.
- Build artifacts are ignored: `bin/`, `bin64/`, `obj/`, `*.o`, `*.res`, `*.zip`, and `src/RA_BuildVer.h`.

## CLI behavior to preserve
- `?` as the system key means auto-detect by extension; numeric equivalent is console ID `91`.
- Multiple filenames/globs disable system auto-detection, so do not use `?` in multi-file mode.
- Wildcards are allowed only in the filename, not the path; on Unix, shell expansion is expected instead of RAHasher wildcard expansion.
- Verbose hash logging is intentionally disabled for multi-file processing.

## Style
- `.editorconfig` requires LF endings and final newlines everywhere.
- `*.h` and `*.cpp` use Latin1 encoding, 2-space indentation, and trimmed trailing whitespace.
