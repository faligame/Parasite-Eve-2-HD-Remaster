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

<p align="center">
  <a href="https://streamable.com/nypzbk"><img src="media/video_thumbnail.jpg" alt="Watch the gameplay video" width="640"></a><br>
  <a href="https://streamable.com/nypzbk"><b>▶ Watch the gameplay video (8 min)</b></a>
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

## Widescreen

Optional 16:9 mode: the scene fills the whole screen while the HUD, text boxes and menus stay exactly where they were.

<table>
  <tr>
    <td><img src="media/screenshots/12_widescreen1.png" alt="Widescreen: MIST armory"></td>
    <td><img src="media/screenshots/13_widescreen2.png" alt="Widescreen"></td>
    <td><img src="media/screenshots/14_widescreen3.png" alt="Widescreen: Dryfield"></td>
  </tr>
</table>

## HD text

<table>
  <tr>
    <td align="center" width="50%"><img src="media/screenshots/15_hdtext_en.png" alt="HD dialogue lettering in English"><br><b>HD dialogue lettering</b></td>
    <td align="center" width="50%"><img src="media/screenshots/16_hdtext_jap.png" alt="HD Japanese menus"><br><b>Japanese menus and item names in HD</b></td>
  </tr>
</table>

---

## Features

### 🖥️ Native PC version
- **Static recompilation** of the original game into a native Windows executable. No emulator required.
- **Vulkan renderer** by default, with every enhancement of the project (OpenGL is still available).
- **High internal resolution**: the 3D scale goes from x1 to **x12** (3840×2880 internal), and the output resolution
  from 1280×720 to **5120×2880**, with presets for the **Steam Deck (1280×800)** and **ultrawide** monitors.
- **NVIDIA DLSS 4 / DLAA** and **AMD FSR 3.1**: temporal reconstruction with native antialiasing (DLAA / FSR Native
  AA) or Quality, Balanced, Performance and Ultra Performance modes. The renderer feeds them real **motion vectors**
  for every moving polygon, so characters stay sharp with no ghosting. FSR works on any graphics card.
- **PGXP geometry precision**: no more wobbling polygons or warping textures, and precise polygon culling so distant
  characters no longer lose triangles.
- **PGXP depth buffer and crack filling**: 3D models no longer flicker or show seams between their polygons at high
  resolution.
- **Flicker-free fullscreen**: borderless fullscreen that never switches the monitor's video mode, even when clicking.
- **60 FPS gameplay** (experimental): the game logic still runs at its original 30 FPS, but the renderer builds an
  intermediate frame with every 3D polygon halfway between two game frames. Characters and enemies move at 60 FPS
  with no added input lag; text, HUD, videos and camera cuts are untouched.
- **FXAA antialiasing** on the game image, leaving text, menus and videos crisp.
- **Widescreen 16:9** (optional): the 4:3 scene is enlarged to fill the screen, trimming a little at the top and
  bottom, and every camera has its own framing so heads and feet stay in view. The HUD, text boxes, the pause menu and
  item examination keep their original 4:3 place and size, and 60 FPS keeps working. The title screen stays in 4:3,
  and the attract demo fills the screen with its logo moved to the corner. The 4:3 mode is untouched.
- **A single launcher**: just open `pe2.exe`. The language you chose decides which engine runs, so the options menu
  always matches the game you are playing.

### ⚙️ Remaster options menu
- Opens from **Options** in the main menu, before you start playing.
- **Redesigned with three tabs**: **Graphics**, **Enhancements** and **Extras**, with option cells, ◄ ► selectors
  and sliders.
- **Original mode**: the game exactly as it was on PlayStation, with a choice of sharp or smooth texture and video
  filtering. **HD mode**: every enhancement enabled.
- **Graphics**: language, mode, resolution (15 presets, from 720p to 5K), 3D scale (x1 to x12, showing the internal
  size), fullscreen, antialiasing (FXAA), reconstruction (Native AA, Quality, Balanced, Performance, Ultra) and upscaler
  (DLSS or FSR 3.1; the ones your graphics card can't run are skipped). Picking a resolution or a reconstruction mode
  sets the recommended 3D scale for you.
- **Enhancements**: HD textures, HD videos, 60 FPS and widescreen.
- **Extras**: unlock every game mode from the start, keyboard setup and save game.
- **Faster loads** in HD mode: doors and camera changes load in a fraction of the time, with music and cutscenes still
  in sync, and the **"Now Loading" screens take about 3 seconds instead of 8**.
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
- **Steady through camera cuts**: holding the stick across several camera changes keeps Aya walking the same way,
  with no back-and-forth between two cameras.
- **Button prompts that match your controller**: menus and the button setup screen show the icons of the last device
  you used, by physical position: **PlayStation, Xbox, Nintendo Switch, Steam Deck or keyboard**, in HD.
- **Keyboard setup** from the Remaster menu, with the assigned keys shown in the game's own menus.

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

### 💾 Saving and single disc
- **Save anywhere**: **L1 + R1 + START** (or **Save game** in the Extras tab) opens the game's own save screen
  wherever you are, outside combat and events, and the save brings you back to that very spot. Western languages
  for now; the Japanese engine comes next.
- **Save states menu** with 12 slots, a thumbnail and the date of each save (**SELECT + R1**).
- **Single-disc experience**: both discs play as one game. When the story moves on to disc 2, or you continue a disc 2
  save from the title screen, the disc is swapped instantly and the disc change screen never appears.
- **Exit** in the pause menu takes you back to the main menu, and the title screen has an **Exit game** option.

### 🌍 One game, six languages
- **English, Spanish, French, German, Italian and Japanese**, selected from the Remaster options menu. The game
  restarts by itself in the chosen language.
- Every language uses the **official text of its own PlayStation release**: dialogues with each language's own
  lettering, item and weapon sheets, memory card messages and menu labels. The few labels the original localizations
  left in English were translated as well, including the weapon sheet tags (RATE, RANGE…) and the Parasite Energy
  names, with short labels where the original box has little room.
- **Japanese: a second engine built on the Japanese release**, with its native menus, item sheets and dialogues.
  Choosing Japanese switches engine by itself; both engines share the save card, the HD pack and every enhancement.
- **HD textures per language**: any image of the pack can have a version for each language, so the title screen is
  shown translated, and every region shows the same publisher screen before the intro.
- Nothing on the discs is modified: each language is a small pack generated from that region's release and applied in
  memory while the game runs.
- On-screen messages (saves, speed, window mode) are shown in a window with the game's own style.

### 🎨 HD Remaster
- **HD pre-rendered backgrounds** at 1440×1080, including the backgrounds streamed in strips during in-game scenes.
- **Text boxes, door transitions, screen shakes and the battle start flash stay in HD.** The original game froze the
  screen at 320×240 in all of them; the remaster keeps the full resolution.
- **HD foreground layers** generated from the HD backgrounds, so objects in front of the characters match the new art.
  Pieces that are an exact cut of the background are now drawn straight from the HD background, with clean edges.
- **Readable text in the backgrounds**: signs, posters and labels that the upscaling had blurred or invented were
  redone so they read as in the original.
- **Remastered textures** for characters, enemies, weapons, HUD and menus. Characters keep their HD textures after
  videos, screen effects and when loading a save state.
- **HD menu font**, with its three palettes (outline, letter and core) redrawn in high resolution.
- **Pixel-exact menu frames**: the lines of every box stay aligned with their panels at any resolution.
- **HD dialogue lettering in all six languages**: every letter of the dialogue boxes and the speaker name tags is
  redrawn in high resolution, per language, and keeps the game's own colours (white, green selection, red and blue
  text). Latin alphabets use the CMU Sans Serif typeface; Japanese uses Noto Sans JP, slanted like the original.
- **Japanese text in HD**: each kanji was identified by reading every sentence in context and checked against the
  shape of the original letter; the few that could not be confirmed keep a clean upscale, so no wrong character ever
  reaches the screen. The Japanese menu, shop and item font is remastered too.
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
| ✅ | High resolution rendering (3D scale up to x12, output up to 5K) and PGXP geometry precision |
| ✅ | **Vulkan renderer** by default |
| ✅ | **NVIDIA DLSS 4 / DLAA** and **AMD FSR 3.1**, with motion vectors |
| ✅ | PGXP depth buffer and crack filling (no flickering models) |
| ✅ | Button prompts for PlayStation, Xbox, Switch, Steam Deck and keyboard |
| ✅ | Remaster menu with Graphics, Enhancements and Extras tabs |
| ✅ | **Save anywhere** (L1 + R1 + START or from the menu) |
| 🚧 | Linux and Steam Deck build (already running, testing on the device pending) |
| ✅ | HD background replacement engine |
| ✅ | HD text boxes, freeze-frames, screen shakes and battle flash |
| ✅ | HD texture replacement engine (per game image, per palette, DuckStation compatible) |
| ✅ | Automatic HD foreground layers |
| ✅ | **HD dialogue lettering** in English, Spanish, French, German, Italian and Japanese |
| ✅ | Japanese menus, shop and item names in HD |
| ✅ | **Widescreen 16:9** (optional), with the HUD and menus kept in 4:3 |
| ✅ | Faster "Now Loading" screens (about 3 s instead of 8) |
| ✅ | Single launcher that picks the engine from the chosen language |
| ✅ | HD textures per language (translated title screen) |
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

**2026-10-15 — Vulkan, DLSS and FSR, a new Remaster menu and controller prompts**
- **Vulkan renderer**, now the default, with every enhancement of the project: HD pack, widescreen, 60 FPS, HD text
  and videos. It is also lighter on the processor than the OpenGL one.
- **NVIDIA DLSS 4 / DLAA and AMD FSR 3.1**: temporal antialiasing at the 3D scale, or reconstruction from a lower
  resolution in Quality, Balanced, Performance and Ultra modes. The 60 FPS polygon matching now also produces real
  **motion vectors**, so moving characters no longer leave a trail.
- **New Remaster menu** in three tabs (Graphics, Enhancements, Extras) with 15 resolution presets up to 5K, including
  Steam Deck and ultrawide, a 3D scale slider up to x12 that suggests the right value for each mode, and the choice
  of upscaler.
- **PGXP depth buffer and crack filling**: models no longer flicker or show seams at high resolution.
- **Controller prompts**: the menus show the buttons of the controller you are using (PlayStation, Xbox, Switch,
  Steam Deck or keyboard), in HD, and the keyboard can be set up from the menu.
- **Unlock every game mode** from the Extras tab, without finishing the game first.
- **Exit** in the pause menu now returns to the main menu, and the title screen can close the game.
- **Widescreen**: the title screen stays in 4:3 and the attract demo fills the screen with its logo in the corner.
- **Modern controls**: holding the stick across several camera cuts no longer makes Aya turn back and forth.
- **HD pack**: readable text on signs and posters, foreground pieces drawn straight from the HD backgrounds, an HD
  menu font, pixel-exact menu frames, and characters that keep their HD textures after videos, effects and save
  states.
- **Fullscreen** no longer blinks to black when clicking: the game tells the driver not to switch to exclusive mode.
- **Save anywhere**: press **L1 + R1 + START** (or use the Extras tab) and the game opens its own save screen, as if you
  were at a phone; loading that save puts Aya right where you saved.
- In testing: a **Linux / Steam Deck** build that already runs.

**2026-09-17 — Widescreen, HD text in every language and a single launcher**
- **Widescreen 16:9**, as an option in the Remaster menu. The 4:3 scene is enlarged to fill the screen and each
  camera has its own framing, so characters keep their heads and feet in view. The HUD, text boxes, the pause menu,
  item examination and effects stay in their original 4:3 place and size, and the 60 FPS mode keeps working. With the
  option off, the game looks exactly as before.
- **HD lettering finished** in Spanish, French, German and Italian, and now **Japanese**: every character used in
  the dialogues was identified by reading each sentence in context and then checked against the shape of the
  original letter. Letters that could not be confirmed keep a clean upscale instead of risking a wrong kanji. The
  Japanese speaker tags and the menu, shop and item font are in HD as well.
- **Faster "Now Loading"**: those screens now take about 3 seconds instead of 8.
- **Translations completed**: weapon sheet tags (RATE, RANGE…), Parasite Energy names and a few menu labels that
  were still in English, shortened where the original box is small. The help text of Exit now says it closes the game.
- **One launcher**: only `pe2.exe` needs to be opened; the chosen language decides which engine runs, and the
  Japanese engine now lives in its own `engine` folder.
- **HD textures per language**: the pack can hold a version of any image for each language, used for the translated
  title screen, and every region now shows the same publisher screen before the intro.

**2026-09-16 — HD dialogue lettering**
- The letters of the dialogue boxes and the speaker name tags are now drawn in **high resolution**. Each room
  ships its own small letter atlas; the remaster recognizes every letter as the game draws it and replaces it
  with a sharp version drawn from the **CMU Sans Serif** typeface, fitted to the exact size and position of the
  original so the text keeps its layout. The game's own palettes are applied live, so white, green, red and blue
  text and the name tags all keep their colours.
- Each language has its own set, with its accents and punctuation (¡ ¿ ñ é ß ä ö ü « » …), and only the set
  of the language you are playing is used.
- English is finished; Spanish, French, German and Italian are generated and in testing. Japanese comes next.

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
| [NVIDIA DLSS](https://developer.nvidia.com/rtx/dlss) | NVIDIA | DLSS 4 / DLAA temporal reconstruction | NVIDIA RTX SDK license |
| [AMD FidelityFX SDK](https://github.com/GPUOpen-LibrariesAndSDKs/FidelityFX-SDK) | AMD | FSR 3.1 temporal reconstruction | MIT |
| [Free Controller & Key Prompts](https://thoseawesomeguys.com/prompts/) | Xelu | Button icons for each controller and the keyboard | CC0 1.0 |
| [PlayStation Specifications (psx-spx)](https://psx-spx.consoledev.net/) | Martin "nocash" Korth and contributors | Hardware and file archive documentation | — |
| [Teko](https://github.com/googlefonts/teko), [Rajdhani](https://github.com/itfoundry/rajdhani), [Barlow](https://github.com/jpt/barlow), [Noto Sans JP](https://github.com/notofonts/noto-cjk) | Indian Type Foundry, Jeremy Tribby, Google and Adobe | Lettering of the Remaster menus | SIL OFL 1.1 |
| [CMU Sans Serif](https://cm-unicode.sourceforge.io/) | Donald Knuth (Computer Modern), Andrey V. Panov (CM-Unicode) | HD dialogue lettering | SIL OFL 1.1 |
| Font replacement tool | u/Over_Transition_8907 | Original HD letter idea and glyph reference used to identify the game's letters | — |
| [Game icon](https://www.steamgriddb.com/) | Ghoulrx (SteamGridDB) | Icon of the game executable | — |

Libraries: [Vulkan](https://www.vulkan.org) (Khronos), [SDL3](https://libsdl.org), [xxHash](https://github.com/Cyan4973/xxHash) (Yann Collet),
[stb_image](https://github.com/nothings/stb) (Sean Barrett), [libchdr](https://github.com/rtissera/libchdr) and [zlib](https://zlib.net).

HD Remaster pack and project: **faligame**.

---

## Legal

This is a non-commercial fan project and is not affiliated with, endorsed by or sponsored by Square Enix.
*Parasite Eve*, *Parasite Eve II* and *FINAL FANTASY VII* are trademarks of Square Enix Co., Ltd. All game content belongs to its respective owners.
NVIDIA and DLSS are trademarks of NVIDIA Corporation. AMD and FidelityFX are trademarks of Advanced Micro Devices, Inc.
PlayStation, Xbox, Nintendo Switch and Steam Deck are trademarks of their respective owners.
This repository does not contain, and will never distribute, game files, BIOS files or copyrighted game assets.
