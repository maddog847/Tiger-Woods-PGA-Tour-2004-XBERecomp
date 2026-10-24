# Tiger Woods PGA Tour 2004 — XBE Recomp

Unofficial native Windows recompilation of the original Xbox version of Tiger Woods PGA Tour 2004. Public beta; original game files required.

Built using [XboxXBERecomp](https://github.com/TGP482/XboxXBERecomp) by [TGP482](https://github.com/TGP482), with title-specific compatibility changes.

## Public Beta

Menus, tutorial progression, normal play, profile saving, video playback, and audio have been exercised during testing. This is an early beta, not a guarantee that every course, mode, or hardware configuration works.

Known issues:
- Tutorial demonstrations and cutscenes may have uneven timing. Tutorial may lag on random shots at rendering higher than 100%.
- Higher render scales can cause slowdowns. Start with the supplied 100% setting.
- Recommend doing initial tutorial at 100% rendering. Beyond that, play was tested up to 300%. Some lag was introduced. 200% was fine and only an occasional lag at times.
  
Further development and ongoing support are not guaranteed. Community improvements are welcome under the applicable included licenses.

## Installation

1. Download **TW2004-Public-Beta-1.zip** from this repository's Releases page.
2. Extract the entire ZIP to a writable folder.
3. Place your extracted original Xbox game files in `assets`, with `default.xbe` directly inside it beside the remaining game files and folders.
4. Open `TW2004.exe` directly. No CMD launcher is needed.

Game files and saves are not included. You must supply your own legally acquired original Xbox copy. Windows PC and PlayStation 2 game files are not compatible. Keep the supplied DLLs beside the EXE.

This build targets one reviewed game executable. Modified or other-region XBEs have not been validated; a version warning does not establish compatibility.

## Controls and settings

Use a compatible game controller for gameplay. Close the game before editing `tw2004-settings.toml`.

- **F11 / Alt+Enter:** toggle windowed and borderless display.
- **Alt+F4:** exit.
- **F12:** save a PNG in `screenshots` beside the EXE.
- The mouse pointer hides over active fullscreen/borderless gameplay and returns in windowed mode or when using the overlay or another app.
  
Output resolution, render percentage, frame cap, VSync, and anisotropic filtering are configurable. Defaults are 1280×720 output, 100% render scale, and a 60 FPS cap. The original game's advertised 480p mode does not limit the PC renderer's resolution. The runtime reports a component/HDTV AV pack without advertising guest 720p.

Save data is stored in `UDATA` on the emulated Xbox E: drive within the local `hdd` folder. Back up the entire `hdd` folder before updating. Keep your existing saves when replacing the executable.

## Source

Download **TW2004-Source-Build_Package.zip** to modify or rebuild the project. Read its `START-HERE.txt`. It includes runtime sources, title configuration, the recompiler, and dependency sources. Game code is generated locally from your own matching XBE; no game assets or generated game code are included.

Use the explicitly named Source-Build package. GitHub's automatic “Source code” downloads contain only whatever has been committed to the repository.

## Credits and notices

Keep the included SDK, Microsoft runtime, and third-party notices with redistributed components. Each component remains subject to its own license.

This is an unofficial community project and is not affiliated with or endorsed by EA, Microsoft, or the PGA Tour.
