# Flare Hub

Flare Hub is a Roblox Islands utility hub focused on autobuilding, farming, movement tools, combat helpers, machinery utilities, teleport options, and general quality-of-life features. It is designed to keep a large amount of functionality inside one script while still being organized through a clean tab-based UI.

## Overview

The main focus of Flare Hub is the autobuild system. It can load saved blueprint JSON files, preview builds with a ghost overlay, place missing blocks, and help automate large builds more efficiently. On top of that, the hub includes extra tools for movement, farming, machinery handling, teleportation, and other utility features.

## Main Features

### Autobuild
- Load and preview saved build files
- Ghost preview / blueprint overlay before placement
- Build full structures from JSON files
- Place only missing blocks
- Snap build position to your current location
- Clear ghost preview when needed
- Optional move-near-block behavior before placing
- Support for block replacement workflows
- Support for cached / resumable build systems depending on version

### Movement
- Movement-related quality-of-life tools
- Float platform support with adjustable offset
- Keybind-based control for certain movement functions

### Farming
- Automation tools for farming-related tasks
- Fish farm support in versions that include it
- Other farm utilities depending on the script build

### Combat
- Mob or boss farming tools in versions that include them
- Bow aura / combat assist style features in some builds

### Machinery
- Utilities for machines and industrial-style setups
- Machine interaction helpers depending on the version

### Teleport / Misc / Settings
- Teleport-related convenience features
- Miscellaneous helper tools
- UI settings, keybinds, theme options, and appearance customization

## How It Works

Flare Hub reads blueprint data from JSON files and uses that data to recreate structures in-game. The build system scans the target area, compares existing blocks against the file, and then attempts to place what is missing. In many versions, this process uses multiple passes and retries to improve placement reliability.

The ghost preview helps line up a structure before committing to the actual placement. This is useful for checking positioning, alignment, and overall scale before starting a full build.

## Typical Autobuild Workflow

1. Open the hub UI.
2. Go to the **Autobuild** tab.
3. Load a saved JSON build file.
4. Preview the structure using the ghost overlay.
5. Adjust the preview position if needed.
6. Use **Build Now** to place the full build, or **Place Missing** to fill in missing parts only.
7. Clear the preview when finished.

## File Format

Blueprints are typically stored as JSON files. Depending on how your version is set up, files may be saved inside folders such as:

```text
autoBuilder/
```

These files usually contain block placement data, positions, and sometimes additional information such as rotation or metadata depending on the version of the system.

## UI Structure

Flare Hub is usually organized into tabs such as:

- Autobuild
- Movement
- Farming
- Combat
- Machinery
- Teleport
- Misc
- Settings

The exact set of tabs can change depending on your current build.

## Warnings

Some features may carry a higher risk than others depending on how they interact with the game. Use caution with automation-heavy features. Test carefully on low-value setups before using anything on important builds, farms, or accounts.

## Performance Notes

Because the script can become very large, some versions may be heavily optimized or refactored to avoid Luau local register limits and reduce lag. If you are editing the source, it is a good idea to keep logic organized into grouped tables, helper functions, or separated scopes where possible.

## Customization

Depending on the build, Flare Hub may support:
- Theme editing
- Neon / purple UI styles
- Window toggle keybinds
- Offset tuning for previews or movement tools
- Feature-specific settings per tab

## Version Notes

Features and behavior may vary between versions of the script. Some builds may include experimental systems such as:
- Cached unfinished builds
- Block replacement editors
- Selection tools
- Region copy / fill tools
- Rotation-aware blueprint placement

## Disclaimer

This project is provided as-is. Compatibility, reliability, and behavior may vary depending on the game version, executor, network conditions, or changes made to the script.

## Credits

Built and maintained by **Xuan**.
