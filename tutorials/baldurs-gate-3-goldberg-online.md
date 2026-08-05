---
game: Baldur's Gate 3
author: patchwizard
version: Goldberg GBE Fork / BG3 Patch 7
date: 2025-11-10
---

# Baldur's Gate 3 — Online Multiplayer via Goldberg Emulator

Step-by-step guide to set up online co-op with friends using Goldberg Steam Emulator without owning the game on Steam.

## Requirements

- Goldberg Steam Emulator GBE Fork ([download](https://github.com/otavepto/gbe_fork))
- Baldur's Gate 3 game files
- All players on same LAN or using Hamachi / ZeroTier for virtual LAN

> ⚠️ **Important:** All players must use the same game version. Mismatched versions will cause connection failures.

## Step 1 — Extract Goldberg

Download the latest Goldberg GBE Fork release and extract it somewhere safe.

```
goldberg_emulator/
  ├── steam_api64.dll
  ├── steam_api.dll
  └── tools/
```

## Step 2 — Find the Steam AppID

BG3's AppID is **1086940**. You'll need this in the next step.

## Step 3 — Configure steam_appid.txt

In the game's root folder, create a file named `steam_appid.txt` containing only:

```
1086940
```

## Step 4 — Replace steam_api64.dll

Copy Goldberg's `steam_api64.dll` into the game's `bin/` directory, replacing the original.

> ℹ️ **Tip:** Back up the original `steam_api64.dll` before replacing it.

## Step 5 — Set up usernames

Each player creates this folder path and file:

```
%appdata%\Goldberg SteamEmu Saves\settings\account_name.txt
```

Write their desired in-game username inside the file.

## Step 6 — Connect

One player hosts by loading a save. Others join via the multiplayer menu using the host's virtual LAN IP.

## Troubleshooting

| Problem | Fix |
|---------|-----|
| Can't see host lobby | Make sure all players are on the same Hamachi network |
| Crash on launch | Verify game files, check you replaced the correct DLL |
| Different game versions | Host and client must match exactly |

## Credits

Guide by **patchwizard** — tested November 2025.
