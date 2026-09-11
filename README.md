<p align="center">
  <img src="media/banner.jpg" alt="Parasite Eve II HD Remaster" width="820">
</p>

<p align="center">
  <b>A native PC version of Parasite Eve II, rebuilt from the original PlayStation game and remastered in high definition.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-in%20development-2ee6d2?style=for-the-badge" alt="Status: in development">
  <img src="https://img.shields.io/badge/platform-Windows-1f6feb?style=for-the-badge" alt="Platform: Windows">
  <img src="https://img.shields.io/badge/fan%20project-non%20commercial-555?style=for-the-badge" alt="Fan project, non commercial">
</p>

<p align="center">
  <a href="README.es.md">🇪🇸 Leer en español</a>
</p>

---

## About the project

**Parasite Eve II HD Remaster** brings Square's 2000 survival horror classic to modern PCs.

This is **not an emulator**. The original PlayStation game code has been statically recompiled into a native Windows
executable, which lets us enhance the game from the inside: sharper 3D, stable geometry, high resolution
pre-rendered backgrounds and a fully remastered texture pack.

This repository is the **public home of the project**: news, screenshots and progress. It does not contain source code,
builds or any game data.

> ⭐ **Star** and 👁️ **Watch** this repository to follow the development.

---

## Screenshots

<table>
  <tr>
    <td><img src="media/screenshots/01_title_screen.png" alt="Title screen"></td>
    <td><img src="media/screenshots/02_akropolis.png" alt="Akropolis Tower"></td>
    <td><img src="media/screenshots/03_mist_shooting_gallery.png" alt="MIST shooting gallery"></td>
  </tr>
  <tr>
    <td><img src="media/screenshots/04_dryfield.png" alt="Dryfield"></td>
    <td><img src="media/screenshots/05_shelter.png" alt="Shelter"></td>
    <td><img src="media/screenshots/06_neo_ark.png" alt="Neo Ark"></td>
  </tr>
  <tr>
    <td><img src="media/screenshots/07_combat_hud.png" alt="Combat and HUD"></td>
    <td><img src="media/screenshots/08_menu_inventory.png" alt="Menu and inventory"></td>
    <td><img src="media/screenshots/09_character_closeup.png" alt="Aya close-up"></td>
  </tr>
</table>

## Before and after

<table>
  <tr>
    <td align="center"><img src="media/comparisons/01_background.webp" alt="Background: PS1 original vs HD"><br><b>Backgrounds</b></td>
    <td align="center"><img src="media/comparisons/02_characters.webp" alt="Characters: PS1 original vs HD"><br><b>Characters</b></td>
  </tr>
  <tr>
    <td align="center"><img src="media/comparisons/03_menu.webp" alt="Menu: PS1 original vs HD"><br><b>Menus and HUD</b></td>
    <td align="center"><img src="media/comparisons/04_geometry.webp" alt="Geometry: PS1 wobble vs PGXP"><br><b>Geometry (PGXP)</b></td>
  </tr>
</table>

---

## Features

### 🖥️ Native PC version
- **Static recompilation** of the original game into a native Windows executable. No emulator required.
- **High internal resolution** rendering for sharp 3D models.
- **PGXP geometry precision**: no more wobbling polygons or warping textures.
- **60 Hz** output with the original **30 FPS** gameplay. **60 FPS coming soon.**

### 🎨 HD Remaster
- **HD pre-rendered backgrounds** at 1440×1080, including the backgrounds streamed in strips during in-game scenes.
- **Text boxes and door transitions stay in HD.** The original game froze the screen at 320×240 whenever a message
  appeared; the remaster keeps the full resolution.
- **HD foreground layers** generated from the HD backgrounds, so objects in front of the characters match the new art.
- **Remastered textures** for characters, enemies, weapons, HUD and menus.
- **Compatible with DuckStation texture packs**: existing `texpage-*` and `vram-write-*` replacements work as-is.

---

## Roadmap

| Status | Feature |
|:---:|---|
| ✅ | Native Windows executable (static recompilation) |
| ✅ | High resolution rendering and PGXP geometry precision |
| ✅ | HD background replacement engine |
| ✅ | HD text boxes and freeze-frames |
| ✅ | HD texture replacement engine (per game image, per palette, DuckStation compatible) |
| ✅ | Automatic HD foreground layers |
| 🚧 | Completing the HD background pack |
| 🚧 | Remastered characters, enemies and weapons |
| 🚧 | Remastered HUD, menus and item icons |
| 🔜 | **60 FPS** gameplay |
| 🔜 | **Native widescreen (16:9)** |
| 🔜 | **Enhanced FMVs** in high resolution |
| 🔜 | Public release |

### HD pack progress

| Asset | Remastered | Total | Progress |
|---|---:|---:|---|
| Pre-rendered backgrounds | 1,328 | 1,759 | ![75%](https://img.shields.io/badge/75%25-2ee6d2?style=flat-square) |
| Game images (characters, HUD, menus, foregrounds) | 864 | 1,453 | ![59%](https://img.shields.io/badge/59%25-2ee6d2?style=flat-square) |

---

## Coming next: widescreen

<p align="center">
  <img src="media/widescreen_preview.png" alt="Widescreen preview" width="100%">
</p>

The goal is a **native 16:9 mode** that renders more of each scene instead of stretching the 4:3 image.
Pre-rendered backgrounds will be extended to fill the wider view.

---

## FAQ

**Is it available for download?**
Not yet. The project is in active development. Watch this repository to be notified of the first release.

**Will I need the original game?**
Yes. You will need your own legal copy of *Parasite Eve II* for PlayStation. No game data will ever be distributed.

**Is this an emulator?**
No. The game code runs natively on your PC after being recompiled from the original PlayStation executable.

**Is the source code available?**
Not at this time.

---

## Legal

This is a non-commercial fan project and is not affiliated with, endorsed by or sponsored by Square Enix.
*Parasite Eve* and *Parasite Eve II* are trademarks of Square Enix Co., Ltd. All game content belongs to its respective owners.
This repository does not contain, and will never distribute, game files, BIOS files or copyrighted game assets.
