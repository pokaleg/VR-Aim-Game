# VR Aim Game

A first person aim training game built in **Unreal Engine 5.6** using **Blueprints**.
Targets appear in the level, the player shoots them with a sniper rifle, and the game tracks the score and shows an end screen when the round is over.

## Features

- **Target system:** custom target actor (`BP_Target`) with its own mesh, materials and a destroyed state when hit
- **Game mode logic:** `GM_TargetGame` controls the round, target spawning and scoring
- **In game HUD:** `WBP_UI` shows live game info such as score
- **End screen:** `WBP_EndScreen` shows the result when the round ends
- **Weapon:** sci-fi sniper rifle with scope, fire effects and audio
- **Player movement and input:** first person character using Enhanced Input (move, look, jump, fire)

## Tech Stack

- Unreal Engine 5.6
- Blueprints (visual scripting)
- UMG (Unreal Motion Graphics) for the UI
- Enhanced Input system

## Project Structure

```
Config/                        Engine, game and input settings
Content/
  FirstPerson/Blueprints/      Character, weapon, projectile, target, game mode and UI blueprints
  FirstPerson/Input/           Input actions and mapping context
  FirstPerson/Maps/            Main game level
  Target/                      Target mesh, materials and textures
  ScifiWeapons/                Sniper rifle mesh, materials, effects and audio
  FPWeapon/, FirstPersonArms/, LevelPrototyping/   Unreal First Person template assets
FirstPersonTemplate.uproject   Unreal project file
```

## How to Run

1. Install **Unreal Engine 5.6** from the Epic Games Launcher
2. Clone this repo:
   ```bash
   git clone https://github.com/pokaleg/VR-Aim-Game.git
   ```
3. Double click `FirstPersonTemplate.uproject` to open it in Unreal Editor
4. Open the map `Content/FirstPerson/Maps/FirstPersonMap`
5. Click **Play**

## Controls

| Action | Key |
|--------|-----|
| Move | W A S D |
| Look | Mouse |
| Jump | Space |
| Fire | Left Mouse Button |

## Credits

- Base character, arms, weapon and level assets come from the **Unreal Engine First Person template**
- Sci-fi sniper rifle assets come from a third party asset pack
