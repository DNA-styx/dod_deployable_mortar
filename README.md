# DoD Deployable Mortar

<img width="1920" height="1080" alt="20D14F~1" src="https://github.com/user-attachments/assets/4696790e-9c84-4416-90c6-53fed237c169" />
<img width="1920" height="1080" alt="206969~1" src="https://github.com/user-attachments/assets/bed3e2fe-d5dd-47b3-b917-80be7aa04d93" />
<img width="1920" height="1080" alt="20E960~1" src="https://github.com/user-attachments/assets/752ae310-f139-427b-b7ff-5570a5994bd6" />
<img width="1920" height="1080" alt="206622~1" src="https://github.com/user-attachments/assets/27e7819d-c32b-4998-945d-50228d5b60c9" />
<img width="1920" height="1080" alt="20E899~1" src="https://github.com/user-attachments/assets/c3591ff2-7fe3-4f1e-aaf9-ab72dea7dfbb" />
<img width="775" height="711" alt="image" src="https://github.com/user-attachments/assets/54ea4685-73ad-4b4e-954f-e172ece6c317" />



## Overview

**DoD Deployable Mortar** is a SourceMod plugin for Day of Defeat: Source that allows players to deploy and operate portable mortars on the battlefield.

## Features

- Deploy and control portable mortars during gameplay
- Menu-based controls to deploy, remove, fire, rotate, and adjust mortar range
- Mortar health, cooldowns, and destruction by enemy fire
- Chat notifications for kills
- HLStatsX support for kills

## Installation

1. **Game Server:**  
   - Extract all files in `GameServer-Files-X.X.XX.zip` attached to the latest release to your  server’s /dod/ directory.

2. **Fast Download Server:**  
   - Extract all files in `FastDL-Files-X.X.XX.zip` into yourFast Download  server.

3. **Restart your server** or reload the plugin to apply changes.

## Usage

- Players say `!mortar` or using sm_mortar in-game to open the mortar menu.
- Mortars can only be placed on open ground, not under cover.
- Menu options:
  - Place/Remove Mortar
  - Fire Mortar
  - Adjust Range (+/-)
  - Rotate Left/Right
- Green smoke appears briefly where the mortar shell will land.
- Fire the mortar by punching/shooting it, or from the menu.
- Mortars can be destroyed by other players.

## HLStatsX Support

- Mortar kills are logged as `mortar_deployable`
- From the HLStatsX admin page, add a new weapon: 
  - Weapon Code: `mortar_deployable`
  - Weapon Name: `Deployable Mortar`
  - Points Modifier: `1` (adjust as you see fit)


## Credits

- Plugin by **Claude.ai guided by DNA.styx**
- Models by The Surgeon  


---

> [GitHub Repository](https://github.com/DNA-styx/dod_deployable_mortar)

