# DoD:S Deployable Mortar

<img width="1920" height="1080" alt="20D14F~1" src="https://github.com/user-attachments/assets/4696790e-9c84-4416-90c6-53fed237c169" />
<img width="1920" height="1080" alt="206969~1" src="https://github.com/user-attachments/assets/bed3e2fe-d5dd-47b3-b917-80be7aa04d93" />
<img width="1920" height="1080" alt="20E960~1" src="https://github.com/user-attachments/assets/752ae310-f139-427b-b7ff-5570a5994bd6" />
<img width="1920" height="1080" alt="206622~1" src="https://github.com/user-attachments/assets/27e7819d-c32b-4998-945d-50228d5b60c9" />
<img width="1920" height="1080" alt="20E899~1" src="https://github.com/user-attachments/assets/c3591ff2-7fe3-4f1e-aaf9-ab72dea7dfbb" />
<img width="775" height="711" alt="image" src="https://github.com/user-attachments/assets/54ea4685-73ad-4b4e-954f-e172ece6c317" />



## Overview

**DoD:S Deployable Mortar** is a SourceMod plugin for Day of Defeat: Source that allows players to deploy and operate portable mortars.

## Features

- Menu-based controls to deploy, remove, fire, rotate, and adjust mortar range
- Team-specific models - Allied and Axis players get different mortars
- Range displayed in metres (20m - 200m, in 10m steps)
- Persistent green smoke and a smoke grenade model mark exactly where the shell will land
- Fire is restricted near objectives, bomb points, spawn areas and off the map, and the menu shows which one is blocking
- Bomb plant points stop being restricted once the bomb has already been detonated
- Mortars have health and can be destroyed by enemy fire, spawning gibs on destruction
- Mortar is destroyed after a configurable number of shots
- Mortar persists when the owner dies but is removed if they change team or go to spectator
- All menu controls disabled when dead and during reload cooldown, re-enabled automatically
- Menus close on round win and map end
- Welcome message on join letting players know the mortar is available
- Chat notifications for kills with team colours
- HLStatsX support for kills and mortar destructions
- Optional admin-only debug beam to visualise where the plugin has detected the target ground

## Installation

1. **Game Server:**  
   - Extract all files in `GameServer-Files-X.X.XX.zip` attached to the latest release to your server's `/dod/` directory.

2. **Fast Download Server:**  
   - Extract all files in `FastDL-Files-X.X.XX.zip` into your Fast Download server.

3. **Restart your server** or reload the plugin to apply changes.

## Usage

- Players say `!mortar` or use `sm_mortar` in-game to open the mortar menu.
- Mortars can only be placed on open ground, not under cover.
- Menu options:
  - Place/Remove Mortar
  - Fire Mortar (shows remaining rounds)
  - Adjust Range (+/- 10m)
  - Rotate Left/Right
- Green smoke and a smoke grenade model mark the shell's landing spot and stay in place until the target is moved.
- Fire the mortar by punching/shooting it, or from the menu.
- Mortars can be destroyed by enemy players.
- Once the shot limit is reached the mortar is automatically destroyed.

## CVars

Saved to `cfg/sourcemod/dod_deployable_mortar.cfg` on first run.

| CVar | Default | Description |
|------|---------|-------------|
| `dod_deployable_mortar_welcome` | `1` | Show welcome message to players on connect (0=off, 1=on) |
| `dod_deployable_mortar_shots` | `5` | Number of shots before mortar is destroyed (0=unlimited) |
| `dod_deployable_mortar_debug` | `0` | Draw a targeting beam visible to admins showing the detected ground position (0=off, 1=on) |

## HLStatsX Support

Mortar events are logged in standard Source log format and ingested by HLStatsX automatically.

From the HLStatsX admin page, add the following:

**Mortar Kill** - add as a Weapon:
- Weapon Code: `mortar_deployable`
- Weapon Name: `Deployable Mortar`
- Points Modifier: `1` (adjust as you see fit)

**Mortar Destroyed** - add as an Action:
- Action Code: `mortar_deployable_destroyed`
- Action Name: `Destroyed a Deployable Mortar`
- Points Modifier: `1` (adjust as you see fit)

## Credits

- Plugin by **Claude.ai guided by DNA.styx**
- Allied mortar model by **The Surgeon**
- Axis mortar model by **Cpt Ukulele**

---

> [GitHub Repository](https://github.com/DNA-styx/dod_deployable_mortar)
