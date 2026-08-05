---
game: Elden Ring
author: rune_seeker
version: OnlineFix v3.1 / ER 1.13
date: 2025-12-02
---

# Elden Ring — Online Multiplayer via OnlineFix

How to use the OnlineFix patch to play Elden Ring online with other cracked game users.

## Requirements

- Elden Ring game files (any release)
- OnlineFix patch for Elden Ring ([onlinefix.me](https://onlinefix.me))
- Game version 1.13

> ⚠️ **EAC Warning:** Easy Anti-Cheat must be bypassed or disabled for OnlineFix to work. Never connect to official servers with this patch.

## Installation

### Step 1 — Download the OnlineFix patch

Get the patch archive from [onlinefix.me](https://onlinefix.me). The archive will contain:
- `OnlineFix64.dll`
- `steam_api64.dll`
- `steam_emu.ini`
- `OnlineFix/` folder

### Step 2 — Configure steam_emu.ini

Open `steam_emu.ini` and set your username:

```ini
[Settings]
PlayerName=YourName
Language=english
SteamId=
```

### Step 3 — Copy files

Copy all files from the patch into your Elden Ring root folder (`ELDEN RING\Game\`).

### Step 4 — Launch

Run `eldenring.exe` directly (not via Steam). You should see the OnlineFix overlay in-game.

## How to Find Games

- Use the in-game summon signs as normal
- Other OnlineFix users will appear in your session

## Troubleshooting

| Problem | Fix |
|---------|-----|
| Black screen on launch | Make sure EAC is bypassed |
| No players found | Check that all players have the same version |
| Crash after 10 min | Copy `oo2core_6_win64.dll` from `_CommonRedist` folder |
