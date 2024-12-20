# Changelog

All notable changes to this project will be documented in this file.

## [24.10-rc.1][] - 2024-11-09

### 🚀 Features

- Build MSI installer with WiX
- Register COM Server and TSF from MSI
- Uninstall NSIS installation from MSI
- Register dll as icon (not working)
- *(msi)* Correctly quote icon path
- *(msi)* Use ITfInputProcessorProfileMgr to register our TS
- *(msi)* Allow upgrade and downgrades
- *(msi)* [**breaking**] Remove nsis installer
- *(prefs)* Enable new keyboard layouts
- Use chewing_ack
- Support config conv engine
- Use 9-patch bitmap to draw candidate window
- Show chi/eng mode toast after manual toggle

### 🐛 Bug Fixes

- Rednering on hidpi device
- Reset composition buffer after toggle chi/eng mode
- Shift key handling
- Only use GetSysColor color index

### 🚜 Refactor

- *(msi)* Use high compression level
- *(libime)* Decouple Window and Dialog
- *(pref)* Decouple with libIME
- Delete unused chewingwrapper
- Draw candidate window with Direct2D
- Draw message window with Direct2D
- Validate client region after drawing
- Remove special immersive mode CandidateWindow
- Use winrt::com_ptr and VersionHelper
- Reimplement MessageWindow in rust
- Hide unused CandidateWindow public methods
- Implement CandidateWindow in rust
- Draw message window background using bitmap
- Cleanup font handling
- Add missing asset
- Simplify candidate window size calculation
- Remove unused DLL registration code (moved to tsfreg)

### 📚 Documentation

- Refresh and add code signing policy info

### ⚙️ Miscellaneous Tasks

- Update dependencies
- Add github actions ci.yaml
- Fix build with Ninja
- Add nightly build workflow
- Introduce dependabot version updates
- Specify LANGUAGES in build script
- Use CMake variable to set MSVC runtime library
- Use CMake variable for enabling LTCG
- Drop redundant macro define
- Drop compiler flag override files
- Reorder override flag
- Remove redundant compile defines
- Specify source code encoding as UTF-8
- Set LANGUAGES property properly
- Add msbuild to path
- Remove libIME as submodule
- Merge libIME back as subdirectory
- Bump libchewing to 0.9.0-rc.3
- Remove cmake minimum version for libIME
- *(libime)* Remove UNICODE defines
- *(libime)* Move files only used by preferences
- Bump libchewing to 0.9.0
- Update signpath action to 1.0
- Simplify cmake files
- Use c++17
- Merge rustlib and libime2
- Fix release workflow
- Bump version to 24.10.258.0
- Bump libchewing to v0.9.0
- Use vcpkg for dependencies
- Update dependencies
- Fix tsfreg artifact location
- Update gitignore
- Remove unused ImeEngine files
- Add git-cliff config file

[24.10-rc.1]: https://github.com/chewing/windows-chewing-tsf/releases/tag/v24.10-rc.1
<!-- generated by git-cliff -->
