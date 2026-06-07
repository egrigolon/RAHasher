# Graph Report - .  (2026-06-07)

## Corpus Check
- 82 files · ~144,697 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 1505 nodes · 3363 edges · 84 communities (72 shown, 12 thin omitted)
- Extraction: 98% EXTRACTED · 2% INFERRED · 0% AMBIGUOUS · INFERRED: 84 edges (avg confidence: 0.79)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Binding Button Input|Binding Button Input]]
- [[_COMMUNITY_Get Delete Shader|Get Delete Shader]]
- [[_COMMUNITY_Memory Read Core|Memory Read Core]]
- [[_COMMUNITY_Core Get Set|Core Get Set]]
- [[_COMMUNITY_Get State Sram|Get State Sram]]
- [[_COMMUNITY_Framebuffer Get Context|Framebuffer Get Context]]
- [[_COMMUNITY_Stbi Load Test|Stbi Load Test]]
- [[_COMMUNITY_Write Stbiw Stbi|Write Stbiw Stbi]]
- [[_COMMUNITY_Stbi Row Memory|Stbi Row Memory]]
- [[_COMMUNITY_Sdl Disc Toggle|Sdl Disc Toggle]]
- [[_COMMUNITY_Stbi Callbacks Load|Stbi Callbacks Load]]
- [[_COMMUNITY_Dialog Get Config|Dialog Get Config]]
- [[_COMMUNITY_Load Save Time|Load Save Time]]
- [[_COMMUNITY_Speex Resampler Get|Speex Resampler Get]]
- [[_COMMUNITY_Core Get Set|Core Get Set]]
- [[_COMMUNITY_Add Write Dialog|Add Write Dialog]]
- [[_COMMUNITY_Stbi Info Header|Stbi Info Header]]
- [[_COMMUNITY_Mic Microphone State|Mic Microphone State]]
- [[_COMMUNITY_Core Get System|Core Get System]]
- [[_COMMUNITY_Bare Core Get|Bare Core Get]]
- [[_COMMUNITY_Core Get Set|Core Get Set]]
- [[_COMMUNITY_Game Get Main|Game Get Main]]
- [[_COMMUNITY_Core Dialog Update|Core Dialog Update]]
- [[_COMMUNITY_Event Get Set|Event Get Set]]
- [[_COMMUNITY_Double Interpolate Product|Double Interpolate Product]]
- [[_COMMUNITY_Core Set Input|Core Set Input]]
- [[_COMMUNITY_Get Fast Forwarding|Get Fast Forwarding]]
- [[_COMMUNITY_Stbi Parse Huffman|Stbi Parse Huffman]]
- [[_COMMUNITY_Mic Core Get|Mic Core Get]]
- [[_COMMUNITY_Game Load Core|Game Load Core]]
- [[_COMMUNITY_Stbi Jpeg Decode|Stbi Jpeg Decode]]
- [[_COMMUNITY_Core Logger Get|Core Logger Get]]
- [[_COMMUNITY_Rhash Hash Error|Rhash Hash Error]]
- [[_COMMUNITY_Stbi Png Compute|Stbi Png Compute]]
- [[_COMMUNITY_Retro Vfs Impl|Retro Vfs Impl]]
- [[_COMMUNITY_Libretro Component Core|Libretro Component Core]]
- [[_COMMUNITY_Cli Port Makefile|Cli Port Makefile]]
- [[_COMMUNITY_Core Reset Allocator|Core Reset Allocator]]
- [[_COMMUNITY_Get State Config|Get State Config]]
- [[_COMMUNITY_Cdrom Get Names|Cdrom Get Names]]
- [[_COMMUNITY_Offset Metadata Frame|Offset Metadata Frame]]
- [[_COMMUNITY_Process Rhash Log|Process Rhash Log]]
- [[_COMMUNITY_Contents Destroy Init|Contents Destroy Init]]
- [[_COMMUNITY_Context Video Core|Context Video Core]]
- [[_COMMUNITY_Mac16 Mult16 Q11|Mac16 Mult16 Q11]]
- [[_COMMUNITY_Create Util Cpp|Create Util Cpp]]
- [[_COMMUNITY_Chd Hash Track|Chd Hash Track]]
- [[_COMMUNITY_Rhash 128Bit 3Ds|Rhash 128Bit 3Ds]]
- [[_COMMUNITY_Application Fsm Memory|Application Fsm Memory]]
- [[_COMMUNITY_Sector Track First|Sector Track First]]
- [[_COMMUNITY_Mac16 Q14 Q15|Mac16 Q14 Q15]]
- [[_COMMUNITY_Stbi Gif Convert|Stbi Gif Convert]]
- [[_COMMUNITY_Audio Core Set|Audio Core Set]]
- [[_COMMUNITY_Microphone Components Fifo|Microphone Components Fifo]]
- [[_COMMUNITY_Core Info Deprecation|Core Info Deprecation]]
- [[_COMMUNITY_Sha256 Hash Final|Sha256 Hash Final]]
- [[_COMMUNITY_Rotation Handler States|Rotation Handler States]]
- [[_COMMUNITY_Mult16 Fixed Spx|Mult16 Fixed Spx]]
- [[_COMMUNITY_About Dialog Destroy|About Dialog Destroy]]
- [[_COMMUNITY_Controller Event Sdl|Controller Event Sdl]]
- [[_COMMUNITY_Dialog Proc Hwnd|Dialog Proc Hwnd]]
- [[_COMMUNITY_Enable Get Uint|Enable Get Uint]]
- [[_COMMUNITY_Namespace Util|Namespace Util]]
- [[_COMMUNITY_Ralibretro Sln Solution|Ralibretro Sln Solution]]
- [[_COMMUNITY_Allocate Destroy Reset|Allocate Destroy Reset]]
- [[_COMMUNITY_Deserialize Get Controller|Deserialize Get Controller]]
- [[_COMMUNITY_Console Group Key|Console Group Key]]
- [[_COMMUNITY_Speex Dsp Libopusfile|Speex Dsp Libopusfile]]
- [[_COMMUNITY_Emulator Report Bug|Emulator Report Bug]]
- [[_COMMUNITY_Init Reset Logger|Init Reset Logger]]
- [[_COMMUNITY_Logger Err Log|Logger Err Log]]
- [[_COMMUNITY_Button Event|Button Event]]
- [[_COMMUNITY_Capture Button Press|Capture Button Press]]
- [[_COMMUNITY_Rumble Set Retro|Rumble Set Retro]]
- [[_COMMUNITY_Input Poll Bare|Input Poll Bare]]
- [[_COMMUNITY_Audio Sample Bare|Audio Sample Bare]]
- [[_COMMUNITY_Environment Bare Core|Environment Bare Core]]
- [[_COMMUNITY_Input State Bare|Input State Bare]]
- [[_COMMUNITY_Video Refresh Bare|Video Refresh Bare]]
- [[_COMMUNITY_Bare Core Load|Bare Core Load]]

## God Nodes (most connected - your core abstractions)
1. `stbi__context` - 69 edges
2. `check()` - 60 edges
3. `stbi_uc` - 41 edges
4. `STBIDEF` - 40 edges
5. `stbi__get8()` - 40 edges
6. `GLuint` - 37 edges
7. `handle()` - 31 edges
8. `InputDialog` - 29 edges
9. `GLenum` - 28 edges
10. `free()` - 28 edges

## Surprising Connections (you probably didn't know these)
- `graphify knowledge graph` --conceptually_related_to--> `CLI macOS/Linux Port Plan`  [INFERRED]
  AGENTS.md → docs/cli-macos-linux-port-plan.md
- `Dialog()` --calls--> `free()`  [INFERRED]
  src/components/Dialog.cpp → src/components/Audio.cpp
- `C/C++ CI` --conceptually_related_to--> `RetroAchievements`  [INFERRED]
  .github/workflows/c-cpp.yml → README.md
- `C/C++ CI` --references--> `Makefile.common`  [INFERRED]
  .github/workflows/c-cpp.yml → AGENTS.md
- `loadFile()` --calls--> `free()`  [INFERRED]
  src/Util.cpp → src/components/Audio.cpp

## Hyperedges (group relationships)
- **CLI porting and verification** — plan_cli_macos_linux_port, readme_rahasher, agents_cli_hasher, workflow_c_cpp_ci [INFERRED 0.78]

## Communities (84 total, 12 thin omitted)

### Community 0 - "Binding Button Input"
Cohesion: 0.05
Nodes (62): array, BindingList, kMaxBindings, SDL_ControllerAxisEvent, SDL_ControllerButtonEvent, SDL_KeyboardEvent, SDL_Keycode, SDL_Scancode (+54 more)

### Community 1 - "Get Delete Shader"
Cohesion: 0.08
Nodes (75): GLbitfield, GLboolean, GLchar, GLclampf, GLfloat, GLsizeiptr, GLvoid, activeTexture() (+67 more)

### Community 2 - "Memory Read Core"
Cohesion: 0.06
Nodes (62): rc_libretro_core_memory_info_t, retro_memory_map, attachToCore(), Core, LoggerComponent, deferredMemoryRead(), dumpDescriptors(), init() (+54 more)

### Community 3 - "Core Get Set"
Cohesion: 0.04
Nodes (4): Core::logCallback(), Core::setMemoryMaps(), fill_bits(), va_list

### Community 4 - "Get State Sram"
Cohesion: 0.08
Nodes (44): destroy(), free(), init(), mix(), reset(), setRate(), write(), Path (+36 more)

### Community 5 - "Framebuffer Get Context"
Cohesion: 0.06
Nodes (40): clear(), clearErrors(), createProgram(), createTexture(), deserializeSettings(), destroy(), draw(), ensureFramebuffer() (+32 more)

### Community 6 - "Stbi Load Test"
Cohesion: 0.12
Nodes (51): stbi__addsizes_valid(), stbi__bmp_info(), stbi__bmp_load(), stbi__bmp_parse_header(), stbi__bmp_test(), stbi__bmp_test_raw(), stbi__convert_format(), stbi__get16le() (+43 more)

### Community 7 - "Write Stbiw Stbi"
Cohesion: 0.11
Nodes (46): va_list, stbi__end_write_file(), stbi_flip_vertically_on_write(), stbi__start_write_callbacks(), stbi__start_write_file(), stbi_write_bmp(), stbi_write_bmp_core(), stbi_write_bmp_to_func() (+38 more)

### Community 8 - "Stbi Row Memory"
Cohesion: 0.09
Nodes (45): load_jpeg_image(), resample_row_1(), stbi__bitcount(), stbi__blinn_8x8(), stbi__clamp(), stbi__compute_y(), stbi__convert_16_to_8(), stbi__copyval() (+37 more)

### Community 9 - "Sdl Disc Toggle"
Cohesion: 0.10
Nodes (39): SDL_MouseButtonEvent, SDL_MouseMotionEvent, SDL_SysWMEvent, SDL_WindowEvent, aboutDialog(), changeCurrentState(), Action, Rotation (+31 more)

### Community 10 - "Stbi Callbacks Load"
Cohesion: 0.10
Nodes (41): FILE, stbi_convert_iphone_png_to_rgb(), stbi__do_zlib(), stbi_failure_reason(), stbi__fopen(), stbi_hdr_to_ldr_gamma(), stbi_hdr_to_ldr_scale(), stbi_image_free() (+33 more)

### Community 11 - "Dialog Get Config"
Cohesion: 0.07
Nodes (25): ConfigDialog::dialogProc(), ConfigDialog::initControls(), ConfigDialog::retrieveData(), deserialize(), deserializeEmulatorSettings(), init(), initializeControllerVariable(), reset() (+17 more)

### Community 12 - "Load Save Time"
Cohesion: 0.15
Nodes (37): FILE, HWND, Logger, string, time_t, deleteFile(), directory(), downloadFile() (+29 more)

### Community 13 - "Speex Resampler Get"
Cohesion: 0.18
Nodes (33): EXPORT, resampler_basic_zero(), speex_alloc(), speex_free(), speex_realloc(), speex_resampler_destroy(), speex_resampler_get_input_latency(), speex_resampler_get_input_stride() (+25 more)

### Community 14 - "Core Get Set"
Cohesion: 0.07
Nodes (15): ConfigComponent, Core::environmentCallback(), Core::getCoreAssetsDirectory(), Core::getFastForwarding(), Core::getSaveDirectory(), Core::getSystemDirectory(), Core::getVariable(), Core::getVariableUpdate() (+7 more)

### Community 15 - "Add Write Dialog"
Cohesion: 0.16
Nodes (26): addButton(), addCheckbox(), addCombobox(), addEditbox(), addLabel(), align(), init(), initControls() (+18 more)

### Community 16 - "Stbi Info Header"
Cohesion: 0.18
Nodes (27): stbi__at_eof(), stbi__build_huffman(), stbi__check_png_header(), stbi__decode_jpeg_header(), stbi__decode_jpeg_image(), stbi__err(), stbi__get16be(), stbi__get8() (+19 more)

### Community 17 - "Mic Microphone State"
Cohesion: 0.10
Nodes (25): closeMic(), destroy(), getMicParams(), getMicState(), init(), Microphone::SDLData, coreRate, deviceId (+17 more)

### Community 19 - "Core Get System"
Cohesion: 0.18
Nodes (22): set, buildSystemMenu(), buildSystemsMenu(), HMENU, handleArgs(), loadCore(), loadGame(), Config (+14 more)

### Community 21 - "Core Get Set"
Cohesion: 0.10
Nodes (12): Core::getCurrentFramebuffer(), Core::getProcAddress(), Core::s_getCurrentFramebuffer(), Core::s_getProcAddress(), Core::setHWRender(), Core::setMessage(), Core::setRotation(), Core::videoRefreshCallback() (+4 more)

### Community 22 - "Game Get Main"
Cohesion: 0.11
Nodes (11): getGameName(), pause(), resume(), CausePause(), CauseUnpause(), HMENU, HWND, GetEstimatedGameTitle() (+3 more)

### Community 23 - "Core Dialog Update"
Cohesion: 0.15
Nodes (15): Dialog, CoreDialog, config, coreNames, loadedCore, logger, modified, numSystems (+7 more)

### Community 24 - "Event Get Set"
Cohesion: 0.11
Nodes (5): Axis, axisEvent(), getJoystickSensitivity(), mouseButtonEvent(), MouseButton

### Community 25 - "Double Interpolate Product"
Cohesion: 0.16
Nodes (16): MULT16_16_P15(), SHL32(), SHR32(), SUB32(), compute_func(), cubic_coef(), main(), resampler_basic_direct_double() (+8 more)

### Community 26 - "Core Set Input"
Cohesion: 0.12
Nodes (10): InputComponent, Core::inputPollCallback(), Core::inputStateCallback(), Core::s_setRumbleCallback(), Core::setControllerInfo(), Core::setInputDescriptors(), Core::setRumble(), Core::step() (+2 more)

### Community 27 - "Get Fast Forwarding"
Cohesion: 0.17
Nodes (13): ConfigDialog(), getAudioWhileFastForwarding(), getFastForwarding(), getFastForwardRatio(), getGameFocusCaptureMouse(), getShowSpeedIndicator(), setFastForwarding(), setSaveDirectory() (+5 more)

### Community 28 - "Stbi Parse Huffman"
Cohesion: 0.30
Nodes (17): stbi__bit_reverse(), stbi__bitreverse16(), stbi__compute_huffman_codes(), stbi__fill_bits(), stbi__parse_huffman_block(), stbi__parse_uncompressed_block(), stbi__parse_zlib(), stbi__parse_zlib_header() (+9 more)

### Community 29 - "Mic Core Get"
Cohesion: 0.24
Nodes (10): Core::s_closeMic(), Core::s_getMicParams(), Core::s_getMicState(), Core::s_openMic(), Core::s_readMic(), Core::s_setMicState(), DummyMicrophone, MicrophoneComponent (+2 more)

### Community 30 - "Game Load Core"
Cohesion: 0.44
Nodes (15): const_string, after(), before(), loadCore(), loadGame(), pauseGame(), pauseGameNoOvl(), quit() (+7 more)

### Community 31 - "Stbi Jpeg Decode"
Cohesion: 0.35
Nodes (16): stbi__build_fast_ac(), stbi__cleanup_jpeg(), stbi__extend_receive(), stbi__free_jpeg_components(), stbi__grow_buffer_unsafe(), stbi__jpeg_decode_block(), stbi__jpeg_decode_block_prog_ac(), stbi__jpeg_decode_block_prog_dc() (+8 more)

### Community 32 - "Core Logger Get"
Cohesion: 0.17
Nodes (12): Core::getDiscLabel(), Core::getDiscPath(), Core::getNeedsFullPath(), Core::getPersistData(), Core::unserialize(), CoreErrorLogger, _errorBuffer, _logger (+4 more)

### Community 33 - "Rhash Hash Error"
Cohesion: 0.16
Nodes (9): unloadGame(), validateHardcoreEnablement(), Core, Logger, string, namespace, libretro(), romLoaded() (+1 more)

### Community 34 - "Stbi Png Compute"
Cohesion: 0.22
Nodes (15): stbi__compute_transparency(), stbi__compute_transparency16(), stbi__create_png_image(), stbi__create_png_image_raw(), stbi__de_iphone(), stbi__do_png(), stbi__expand_png_palette(), stbi__get_chunk_header() (+7 more)

### Community 35 - "Retro Vfs Impl"
Cohesion: 0.15
Nodes (14): retro_vfs_file_close_impl(), retro_vfs_file_flush_impl(), retro_vfs_file_get_path_impl(), retro_vfs_file_handle, fp, orig_path, retro_vfs_file_open_impl(), retro_vfs_file_read_impl() (+6 more)

### Community 36 - "Libretro Component Core"
Cohesion: 0.21
Nodes (8): libretro(), ConfigComponent(), LoggerComponent(), VideoContextComponent(), libretro(), namespace, class, namespace

### Community 37 - "Cli Port Makefile"
Cohesion: 0.18
Nodes (13): CLI hasher, graphify knowledge graph, GUI/libretro app, Makefile.common, port/cli-chd-support, CLI macOS/Linux Port Plan, port/cli-posix-build, Command Line Arguments (+5 more)

### Community 38 - "Core Reset Allocator"
Cohesion: 0.17
Nodes (9): AllocatorComponent, Core::destroy(), Core::loadCore(), Core::loadGame(), Core::reset(), Core::resetGame(), Core::setKeyboardCallback(), Core::strdup() (+1 more)

### Community 39 - "Get State Config"
Cohesion: 0.24
Nodes (12): string, destroy(), getConfigPath(), getCoreConfigPath(), getStatePath(), init(), loadConfiguration(), loadState() (+4 more)

### Community 40 - "Cdrom Get Names"
Cohesion: 0.26
Nodes (7): cdrom_get_cd_names(), cdrom_get_cd_names_m3u(), Logger, string, vector, namespace, util()

### Community 41 - "Offset Metadata Frame"
Cohesion: 0.17
Nodes (12): metadata, frame_offset, frames, pad, pgsub, pgtype, postgap, pregap (+4 more)

### Community 42 - "Process Rhash Log"
Cohesion: 0.38
Nodes (9): printf(), string, find_console_id(), main(), process_file(), process_files(), process_iterated_file(), rhash_log() (+1 more)

### Community 43 - "Contents Destroy Init"
Cohesion: 0.27
Nodes (8): contents(), iterate(), log(), peek(), read(), write(), Iterator, string

### Community 44 - "Context Video Core"
Cohesion: 0.18
Nodes (5): init(), VideoContextComponent(), SDL_Window, LoggerComponent, class

### Community 45 - "Mac16 Mult16 Q11"
Cohesion: 0.36
Nodes (9): MAC16_16(), MAC16_32_Q11(), MAC16_32_Q15(), MULT16_16(), MULT16_32_Q11(), MULT16_32_Q15(), resampler_basic_direct_single(), spx_word16_t (+1 more)

### Community 46 - "Create Util Cpp"
Cohesion: 0.29
Nodes (10): GLenum, GLint, GLsizei, GLuint, LoggerComponent, createFramebuffer(), createProgram(), createShader() (+2 more)

### Community 47 - "Chd Hash Track"
Cohesion: 0.29
Nodes (9): chd_file, metadata_t, rc_hash_iterator_t, rc_hash_find_chd_track(), rc_hash_get_chd_metadata(), rc_hash_handle_chd_close_track(), rc_hash_handle_chd_open_track(), rc_hash_handle_chd_read_sector() (+1 more)

### Community 48 - "Rhash 128Bit 3Ds"
Cohesion: 0.35
Nodes (10): string, initHash3DS(), rhash_3ds_lookup_cia_normal_key(), rhash_3ds_lookup_ncch_normal_key(), rhash_3ds_normalize_keys(), rhash_add_128bit(), rhash_print_key(), rhash_read_128bit_hex() (+2 more)

### Community 49 - "Application Fsm Memory"
Cohesion: 0.24
Nodes (6): class, Application(), Fsm(), class, class, Memory()

### Community 50 - "Sector Track First"
Cohesion: 0.20
Nodes (10): chd_track_handle_t, file, first_frame, first_sector, frames_in_track, frames_per_hunk, hunkmem, hunknum (+2 more)

### Community 51 - "Mac16 Q14 Q15"
Cohesion: 0.44
Nodes (9): DIV32_16(), MAC16_32_Q14(), MAC16_32_Q15(), MAX16(), MULT16_32_Q14(), MULT16_32_Q15(), PDIV32_16(), spx_word16_t (+1 more)

### Community 52 - "Stbi Gif Convert"
Cohesion: 0.27
Nodes (10): stbi__compute_y_16(), stbi__convert_8_to_16(), stbi__convert_format16(), stbi__jpeg_dequantize(), stbi__jpeg_finish(), stbi__load_and_postprocess_16bit(), stbi__out_gif_code(), stbi__process_gif_raster() (+2 more)

### Community 53 - "Audio Core Set"
Cohesion: 0.22
Nodes (6): AudioComponent, Core::audioSampleBatchCallback(), Core::audioSampleCallback(), Core::handleSystemAVInfoChanged(), Core::setGeometry(), DummyAudio

### Community 54 - "Microphone Components Fifo"
Cohesion: 0.25
Nodes (6): Components, Fifo(), MicrophoneComponent(), Core::init(), class, class

### Community 55 - "Core Info Deprecation"
Cohesion: 0.22
Nodes (9): CoreInfo, deprecationMessage, extensions, filename, filetime, name, servertime, systems (+1 more)

### Community 56 - "Sha256 Hash Final"
Cohesion: 0.44
Nodes (6): SHA256_final(), SHA256_hash(), SHA256_init(), SHA256_Transform(), SHA256_update(), SHA256_CTX

### Community 57 - "Rotation Handler States"
Cohesion: 0.25
Nodes (6): setRotationChangedHandler(), RotationHandler, reset(), virtual, class, States()

### Community 58 - "Mult16 Fixed Spx"
Cohesion: 0.32
Nodes (4): MULT16_32_Q14(), MULT16_32_Q15(), spx_word16_t, spx_word32_t

### Community 60 - "Controller Event Sdl"
Cohesion: 0.52
Nodes (7): addController(), processEvent(), removeController(), KeyBinds, SDL_Event, SDL_JoystickID, VideoComponent

### Community 61 - "Dialog Proc Hwnd"
Cohesion: 0.33
Nodes (6): dialogProc(), HWND, LPARAM, UINT, virtual, WPARAM

### Community 62 - "Enable Get Uint"
Cohesion: 0.40
Nodes (6): UINT, enableItems(), enableRecent(), updateMenu(), getSystemName(), s_getCoreName()

### Community 63 - "Namespace Util"
Cohesion: 0.33
Nodes (4): Gl(), namespace, GlUtil(), namespace

### Community 64 - "Ralibretro Sln Solution"
Cohesion: 0.40
Nodes (3): libchdr, RAHasher, RALibretro

### Community 65 - "Allocate Destroy Reset"
Cohesion: 0.50
Nodes (3): allocate(), reset(), virtual

### Community 66 - "Deserialize Get Controller"
Cohesion: 0.40
Nodes (5): deserialize(), getControllerNames(), serialize(), string, vector

### Community 67 - "Console Group Key"
Cohesion: 0.40
Nodes (5): console_t, group, id, key, name

### Community 68 - "Speex Dsp Libopusfile"
Cohesion: 1.00
Nodes (4): libopusfile, Opus, SpeexDSP 1.2rc3, SpeexDSP

### Community 70 - "Emulator Report Bug"
Cohesion: 0.67
Nodes (3): Report an emulator bug, Issue template config, Suggest an emulator feature

### Community 71 - "Init Reset Logger"
Cohesion: 0.67
Nodes (3): init(), reset(), LoggerComponent

## Knowledge Gaps
- **196 isolated node(s):** `RALibretro`, `RAHasher`, `libchdr`, `rc_libretro_core_memory_info_t`, `retro_memory_map` (+191 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **12 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `free()` connect `Get State Sram` to `Rhash Hash Error`, `Retro Vfs Impl`, `Framebuffer Get Context`, `Get State Config`, `Sdl Disc Toggle`, `Process Rhash Log`, `Load Save Time`, `Add Write Dialog`, `Chd Hash Track`, `Core Get System`?**
  _High betweenness centrality (0.132) - this node is a cross-community bridge._
- **Why does `retro_vfs_file_close_impl()` connect `Retro Vfs Impl` to `Core Get Set`, `Get State Sram`?**
  _High betweenness centrality (0.069) - this node is a cross-community bridge._
- **Why does `Components` connect `Microphone Components Fifo` to `Cdrom Get Names`, `Get Fast Forwarding`, `Context Video Core`, `Rotation Handler States`, `About Dialog Destroy`?**
  _High betweenness centrality (0.034) - this node is a cross-community bridge._
- **What connects `RALibretro`, `RAHasher`, `libchdr` to the rest of the system?**
  _196 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Binding Button Input` be split into smaller, more focused modules?**
  _Cohesion score 0.05123456790123457 - nodes in this community are weakly interconnected._
- **Should `Get Delete Shader` be split into smaller, more focused modules?**
  _Cohesion score 0.08091908091908091 - nodes in this community are weakly interconnected._
- **Should `Memory Read Core` be split into smaller, more focused modules?**
  _Cohesion score 0.05547785547785548 - nodes in this community are weakly interconnected._