# BGA Mode 0.1.27

BGA Mode is a Unity Mod Manager mod for ADOFAI that hides the playable chart, player elements, and gameplay HUD while keeping the background and VFX visible.

## Features

- Hides playable chart tiles, planets, tails, judgments, and gameplay HUD
- Keeps backgrounds, camera movement, filters, flashes, particles, and custom UI VFX
- Keeps the lobby and custom-level selection screens usable
- Keeps the chart visible while editing and applies BGA Mode only during editor playback
- Optional hiding for effect-created tiles
- Optional hiding for effect planets and planet-anchored decorations
- Optional hit-sound muting
- Optional muting for other gameplay sound effects and custom Play Sound events
- Top-right Build Text hiding and custom text
- Korean font support for custom Build Text
- Persistent settings
- One-click Korean/English switching in Mod Manager

Music and Mod Manager/menu interface sounds are not affected by the gameplay sound options.

## Download

Download `BgaMode-0.1.27.zip` from the [public download page](https://github.com/cgwoo0704/ADOFAI-BGA-Mode-Downloads/releases/latest). This repository contains installation packages and documentation only. GitHub's automatically generated `Source code` archives also contain no mod source code and are not installation packages.

## Installation

1. Install Unity Mod Manager for ADOFAI.
2. Extract the release ZIP into the game's `Mods` folder.
3. Confirm this folder structure:

```text
Mods/
└─ BgaMode/
   ├─ BgaMode.dll
   ├─ Info.json
   ├─ README.md
   ├─ README_KO.md
   ├─ README_EN.md
   ├─ CHANGELOG.md
   └─ LICENSE
```

4. Fully close and restart the game.
5. Open Mod Manager and confirm that `BGA Mode 0.1.27` is active.

## Language

Expand `BGA Mode` in Mod Manager and click either `한국어` or `English`. The interface changes immediately without restarting the game. The selected language is saved for future launches.

The mod name, Build Text entered by the user, technical hook names, and diagnostic log entries are not translated.

## Usage

Enable `BGA Mode` to reveal the following options:

- `Also hide effect-created tiles`
- `Also hide effect planets and planet-anchored decorations`
- `Mute hit sounds`
- `Mute other gameplay sound effects`

Build Text options remain available independently from BGA Mode:

- `Hide top-right Build Text`
- `Use custom Build Text`
- `Custom text`

The custom text is empty on a fresh install. `Reset Build Text settings` disables hiding and custom text, then clears the saved text.

Changes are saved automatically, so there is no separate text save button. Settings are stored outside the mod installation folder and remain when a release ZIP is installed over the existing mod.

## Compatibility status

When BGA Mode is enabled, Mod Manager displays one of these states:

- `Ready`: editor, floor, effect, and sound hooks were installed
- `Some features need attention`: one or more optional game methods could not be found or patched
- `Hook installation failed`: an unexpected error occurred during initial hook setup

If the status is not Ready, check the `BGA Mode compatibility` entry in the Mod Manager Logs tab.

## Updating

Close the game and replace the files in `Mods/BgaMode` with the files from the new release. User settings are stored separately and normally remain intact.

## Uninstalling

Close the game and remove the `Mods/BgaMode` folder. The mod does not modify chart files or gameplay timing data.

## Bug reports

Use the [GitHub bug report form](https://github.com/cgwoo0704/ADOFAI-BGA-Mode-Downloads/issues/new/choose). A GitHub account is required. Reports are public, so do not include private information.

Please include:

- BGA Mode version
- ADOFAI build and Unity Mod Manager version
- The `BGA Mode compatibility` line from the Logs tab
- Whether the issue occurred in the lobby, editor, editor playback, or regular gameplay
- The actions immediately before the issue
- A short video or screenshot when possible

## Tested environment

- Windows 11
- ADOFAI Alpha Build
- Unity Mod Manager 0.32.5.0

ADOFAI alpha updates may affect compatibility.

## Author and license

- Author: 최건오사임
- License: MIT License

BGA Mode is an unofficial fan-made mod and is not an official feature or mod from 7th Beat Games.
