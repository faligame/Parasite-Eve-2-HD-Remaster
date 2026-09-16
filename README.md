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

## In-game menus

Both menus are drawn with the game's own panels, frames, font and cursor, so they feel like part of the original game.

<table>
  <tr>
    <td align="center" width="50%"><img src="media/screenshots/10_extra_options.png" alt="Remaster options menu"><br><b>Remaster options</b><br>Opens from <b>Options</b> in the main menu</td>
    <td align="center" width="50%"><img src="media/screenshots/11_saveload_states_menu.png" alt="Save states menu"><br><b>Save states</b><br><b>SELECT + R1</b> on the controller</td>
  </tr>
</table>

---

## Features

### 🖥️ Native PC version
- **Static recompilation** of the original game into a native Windows executable. No emulator required.
- **High internal resolution** rendering for sharp 3D models, up to **4K**.
- **PGXP geometry precision**: no more wobbling polygons or warping textures, and precise polygon culling so distant
  characters no longer lose triangles.
- **60 FPS gameplay** (experimental): the game logic still runs at its original 30 FPS, but the renderer builds an
  intermediate frame with every 3D polygon halfway between two game frames. Characters and enemies move at 60 FPS
  with no added input lag; text, HUD, videos and camera cuts are untouched.
- **FXAA antialiasing** on the game image, leaving text, menus and videos crisp.

### ⚙️ Remaster options menu
- Opens from **Options** in the main menu, before you start playing.
- **Original mode**: the game exactly as it was on PlayStation, with a choice of sharp or smooth texture and video
  filtering. **HD mode**: every enhancement enabled.
- Internal resolution (**Original, HD, Full HD, 4K**), HD textures, HD videos, FXAA, scanlines, 60 FPS, fullscreen and
  window size.
- **Faster loads** in HD mode: doors and camera changes load in a fraction of the time, with music and cutscenes still
  in sync.
- When a change needs a restart, the game **saves it and restarts by itself**.
- **Drawn in six languages**: the menu translates itself on the fly while you pick the language. Its lettering is
  generated from the Teko, Rajdhani, Barlow and Noto Sans JP typefaces, with the PlayStation button glyphs in color,
  and every action has its own sound.

### 🎮 Modern controls
- **Left stick: modern controls.** Aya walks in the direction you push, relative to the camera, as in the
  *Resident Evil* remake. Turns are instant, pushing the stick all the way makes her run, and when the camera cuts
  the direction is kept until you move the stick, so she never spins round on a scene change.
- **D-pad: classic tank controls**, untouched. Both work at the same time, with no setting to choose.
- **Also in combat**: with the weapon ready, the stick moves Aya instantly; release it and the game's own auto-aim
  turns her back to the locked target, ready to shoot. Starting to walk, run or lower the weapon no longer waits
  for the long animation blends.

### ⚡ Game boosters
Inspired by the quality-of-life boosters Square Enix added to its modern re-releases of classics like
**FINAL FANTASY VII**, they are toggled at any time with the controller, and every active booster stays on screen as an
icon in the top-right corner.

<table>
  <tr>
    <td align="center" width="33%"><img src="media/icons/speed_x4.png" alt="Speed x4" width="80"><br><b>Speed x4</b><br>Hold <b>L2</b> (or Tab on the keyboard)</td>
    <td align="center" width="33%"><img src="media/icons/hp_infinite.png" alt="Infinite HP" width="80"><br><b>Infinite HP</b><br><b>SELECT + ✕</b></td>
    <td align="center" width="33%"><img src="media/icons/mp_infinite.png" alt="Infinite MP" width="80"><br><b>Infinite MP</b><br><b>SELECT + □</b></td>
  </tr>
</table>

Also available: **SELECT + △** keeps your BP at the maximum and **SELECT + ○** keeps EXP at 6000 to upgrade Aya.

### 💾 Save states and single disc
- **Save states menu** with 12 slots, a thumbnail and the date of each save (**SELECT + R1**).
- **Single-disc experience**: both discs play as one game. When the story moves on to disc 2, or you continue a disc 2
  save from the title screen, the disc is swapped instantly and the disc change screen never appears.
- **Exit** in the pause menu closes the game.

### 🌍 One game, six languages
- **English, Spanish, French, German, Italian and Japanese**, selected from the Remaster options menu. The game
  restarts by itself in the chosen language.
- Every language uses the **official text of its own PlayStation release**: dialogues with each language's own
  lettering, item and weapon sheets, memory card messages and menu labels. The few labels the original localizations
  left in English were translated as well.
- **Japanese: a second engine built on the Japanese release**, with its native menus, item sheets and dialogues.
  Choosing Japanese switches engine by itself; both engines live in the same folder and share the save card, the
  HD pack and every enhancement.
- Nothing on the discs is modified: each language is a small pack generated from that region's release and applied in
  memory while the game runs.
- On-screen messages (saves, speed, window mode) are shown in a window with the game's own style.

### 🎨 HD Remaster
- **HD pre-rendered backgrounds** at 1440×1080, including the backgrounds streamed in strips during in-game scenes.
- **Text boxes, door transitions, screen shakes and the battle start flash stay in HD.** The original game froze the
  screen at 320×240 in all of them; the remaster keeps the full resolution.
- **HD foreground layers** generated from the HD backgrounds, so objects in front of the characters match the new art.
- **Remastered textures** for characters, enemies, weapons, HUD and menus.
- **High resolution cinematics**: every FMV frame is recognized as the game decodes it and replaced by its high
  resolution version (for example, upscaled with AI), so the videos keep the game's own audio and timing and can never
  go out of sync. The original videos are still available from the options menu.
- **Compatible with DuckStation texture packs**: existing `texpage-*` and `vram-write-*` replacements work as-is.
- **Made for texture artists**: replacements are named after the game's own files (`bs_N.png` backgrounds,
  `pe2img_N.png` images), the pack **reloads while the game is running** (save a PNG and see it in-game instantly),
  and a color gallery of every image on the disc plus an identification tool for DuckStation dumps keep track of what
  is done, in progress and missing.

---

## Roadmap

| Status | Feature |
|:---:|---|
| ✅ | Native Windows executable (static recompilation) |
| ✅ | High resolution rendering (up to 4K) and PGXP geometry precision |
| ✅ | HD background replacement engine |
| ✅ | HD text boxes, freeze-frames, screen shakes and battle flash |
| ✅ | HD texture replacement engine (per game image, per palette, DuckStation compatible) |
| ✅ | Automatic HD foreground layers |
| ✅ | **60 FPS** gameplay by polygon interpolation (experimental) |
| ✅ | Precise polygon culling (PGXP) |
| ✅ | FXAA antialiasing |
| ✅ | **Six languages**: English, Spanish, French, German, Italian and Japanese dialogues |
| ✅ | **Japanese engine** with native menus (second executable, same folder) |
| ✅ | **Modern controls** on the stick (camera relative) alongside classic controls on the D-pad |
| ✅ | Remaster menu in six languages with new lettering and sounds |
| 🔜 | Installer that builds the game from your own discs, so no game data is ever distributed |
| ✅ | **Remaster options menu** with Original and HD modes |
| ✅ | **Game boosters**: speed x4, infinite HP and MP, max BP and EXP |
| ✅ | **Save states menu** with thumbnails |
| ✅ | **Single-disc experience** (no disc change screen) |
| ✅ | Faster loads on doors and camera changes |
| ✅ | Hot reload of the HD pack and disc-named textures for artists |
| 🚧 | Completing the HD background pack |
| 🚧 | Remastered characters, enemies and weapons |
| 🚧 | Remastered HUD, menus and item icons |
| ✅ | **High resolution cinematics** engine (FMVs replaced frame by frame, always in sync) |
| 🚧 | Upscaling every FMV to high resolution |
| 🔜 | Public release |

### HD pack progress

| Asset | Remastered | Total | Progress |
|---|---:|---:|---|
| Pre-rendered backgrounds | 1,328 | 1,759 | ![75%](https://img.shields.io/badge/75%25-2ee6d2?style=flat-square) |
| Game images (characters, HUD, menus, foregrounds) | 864 | 1,453 | ![59%](https://img.shields.io/badge/59%25-2ee6d2?style=flat-square) |

---

## News

**2026-09-16 — Modern controls, Japanese engine and a new Remaster menu**
- **Modern controls**: the left stick moves Aya relative to the camera, as in the *Resident Evil* remake, with
  instant turns and running when pushed all the way; on a camera cut the direction is kept until you move the
  stick. The D-pad keeps the classic tank controls, and both work at once. It also works in combat: the stick moves
  Aya with the weapon ready and, when released, the game's auto-aim brings her back onto the target. The animation
  blends when starting to walk, run or lower the weapon were shortened so she responds right away.
- **Japanese engine**: the Japanese release now runs as a second engine with its native menus, item sheets and
  dialogues, and every enhancement of the project (HD pack, cinematics, 60 FPS, single disc, boosters). Choosing
  Japanese in the options menu switches engine automatically; both share one folder and one save card.
- **Remaster menu redone**: language first, translated on the fly while you pick it, new lettering generated from
  the Teko, Rajdhani, Barlow and Noto Sans JP typefaces, PlayStation button glyphs, plain frames, and sounds for
  opening, moving, choosing and saving. The save states menu and the on-screen messages follow the chosen language.

**2026-09-16 — Six languages in one game**
- The project moved to the **US release as its base**, and every other language is imported on top of it: **Spanish,
  French, German, Italian** and **Japanese**, chosen from the Remaster options menu.
- Each language brings the **official text of its own PlayStation release**: the dialogues, with each language's own
  lettering, the item and weapon sheets, the memory card messages and the menu labels. Where the original localizations
  kept some labels in English, they were translated too. A handful of rooms whose dialogue logic differs between
  regions use the US logic with the localized text, so nothing is left untranslated.
- **Japanese dialogues** did not fit on the US disc (kanji lettering is two to three times larger), so the letter
  images are delivered straight into video memory as the game loads each room. Japanese menus and item sheets use a
  different text engine; a dedicated build on the Japanese executable has started.
- Under the hood: the translation engine now scans each loaded module once instead of once per text, which removes the
  stutter on loading screens; and loading a save game with a translated language, which used to freeze on "Now
  loading", is fixed.

**2026-09-15 — Remaster options menu, game boosters, save states and a single disc**
- **Remaster options menu** inside the game, opened from Options in the main menu and drawn with the game's own style:
  Original or HD mode, resolution up to 4K, HD textures and videos, FXAA, scanlines, 60 FPS and window options. The game
  restarts by itself to apply changes that need it.
- **Game boosters** inspired by Square Enix's re-releases such as FINAL FANTASY VII: hold L2 for speed x4, and toggle
  infinite HP, infinite MP, max BP and EXP with SELECT and the face buttons. Active boosters are shown as icons.
- **Save states menu** redesigned with the game's look: 12 slots with a thumbnail and date.
- **Single-disc experience**: the runtime swaps discs by itself before the game asks for it, so the disc change screen
  is gone, also when continuing a disc 2 save or loading a save state.
- **High resolution cinematics**: FMVs are replaced frame by frame by their high resolution versions while the game
  keeps playing its own audio, so they stay perfectly in sync.
- **HD everywhere**: FXAA antialiasing, the black and white battle start flash and boss screen shakes now keep the full
  resolution, and in-game cutscenes stay in sync with faster door and camera loads.

**2026-09-14 — 60 FPS, precise culling, Spanish menus and tools**
- **60 FPS gameplay** (experimental). Forcing the game to run at 60 doubled its speed, so instead the renderer records
  every polygon of each game frame and composes an intermediate frame with the 3D geometry halfway between two frames.
  It matches polygons by texture coordinates, keeps text and UI still, and switches itself off on camera cuts, loads,
  frozen screens and videos. No extra input latency.
- **Precise culling**: distant characters lost triangles because the PlayStation decides visibility on integer
  coordinates. The GTE now keeps sub-pixel precision through the game's own vertex reloads, and every culling decision
  is made with it.
- **Spanish menus and item sheets**: the last English strings (menu labels, ammo and armor sheets) are translated in
  memory and on the fly when read from the disc, so the game files stay untouched.
- **For artists**: the HD pack is now split into *final*, *in progress* and *missing*, files use the disc's own names,
  and the game reloads any PNG the moment it is saved.

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

## Credits

This project stands on the shoulders of these amazing projects and people:

| Project | Author | Used for | License |
|---|---|---|---|
| [PSXRecomp](https://github.com/mstan/psxrecomp) | Matthew Stan | The PlayStation static recompiler and hardware-accurate runtime this port is built on | PolyForm Noncommercial 1.0.0 |
| [Parasite Eve II Decompilation](https://github.com/GabeRealB/parasite-eve-2-decomp) | GabeRealB and contributors | Game file formats, asset extraction tools, symbols and room names | CC0 1.0 |
| [DuckStation](https://github.com/stenzek/duckstation) | Stenzek | Reference for texture replacement naming and MDEC decoding, so DuckStation texture packs work as-is | CC BY-NC-ND 4.0 |
| [Beetle PSX](https://github.com/libretro/beetle-psx-libretro) | libretro, based on Mednafen | Accuracy reference used by PSXRecomp | GPL-2.0 |
| PGXP | iCatButler | Original geometry precision technique | — |
| FXAA | Timothy Lottes (NVIDIA) | Original fast approximate antialiasing technique | — |
| [PlayStation Specifications (psx-spx)](https://psx-spx.consoledev.net/) | Martin "nocash" Korth and contributors | Hardware and file archive documentation | — |
| [Teko](https://github.com/googlefonts/teko), [Rajdhani](https://github.com/itfoundry/rajdhani), [Barlow](https://github.com/jpt/barlow), [Noto Sans JP](https://github.com/notofonts/noto-cjk) | Indian Type Foundry, Jeremy Tribby, Google and Adobe | Lettering of the Remaster menus | SIL OFL 1.1 |

Libraries: [SDL3](https://libsdl.org), [xxHash](https://github.com/Cyan4973/xxHash) (Yann Collet),
[stb_image](https://github.com/nothings/stb) (Sean Barrett), [libchdr](https://github.com/rtissera/libchdr) and [zlib](https://zlib.net).

HD Remaster pack and project: **faligame**.

---

## Legal

This is a non-commercial fan project and is not affiliated with, endorsed by or sponsored by Square Enix.
*Parasite Eve*, *Parasite Eve II* and *FINAL FANTASY VII* are trademarks of Square Enix Co., Ltd. All game content belongs to its respective owners.
This repository does not contain, and will never distribute, game files, BIOS files or copyrighted game assets.
