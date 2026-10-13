[日本語](README.md)

# SETOLIA

Setlist plugin for OBS Studio

## Main Features

- Synchronized timestamp with the streaming time
- Automatic song number increment
- Real-time clock display
- Shortcut button to [lyrics search site](<(https://utaten.com)>)
- Button to add pre-configured browser source
- Support custom template
- Supports operation from Stream Deck

## Installation

Binaries for Windows, MacOS, and Linux are available in the [Releases](https://github.com/Yagami-Huki/setolia/releases) section.

Also, the latest installer for Windows is available at [Booth](https://logicbox.booth.pm/items/7541386).

### Portable OBS

Extract OBS into the `portable` folder and run `scripts/deploy_to_portable.ps1`.

## Building

Requirements: Visual Studio 2026 (Desktop development with C++ workload), CMake 3.28+

Dependencies are downloaded automatically during CMake configure.

```powershell
cmake --preset windows-x64
cmake --build --preset windows-x64
cmake --install build_x64
```

The default install location of `cmake --install` is `C:\ProgramData\obs-studio\plugins\setolia`.

For macOS / Linux, use the `macos` / `ubuntu-x86_64` presets in `CMakePresets.json`.

## Usage

The English version of the user manual is currently under preparation.

Please refer to the Japanese manual available at [Booth](https://logicbox.booth.pm/items/7541386).

## License & Acknowledgements

This software is licensed under the GPL-3.0 License.

This project was developed using the [obs-plugintemplate](https://github.com/obsproject/obs-plugintemplate) from the [OBS Project](https://github.com/obsproject).

Also, the standard templates included with this software are licensed under the MIT License.
