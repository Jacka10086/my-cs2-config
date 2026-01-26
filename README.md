# My CS2 Config

Personal Counter-Strike 2 configuration files collection.

## 📁 File Description

### Core Config Files

- **`autoexec.cfg`** - Auto-execute config file, automatically loaded when game starts
- **`x.cfg`** - Main config file, contains sensitivity, crosshair, viewmodel settings, etc. (for local/offline use)
- **`x_online.cfg`** - Community server config file, removes buy commands that may be restricted on servers
- **`buy.cfg`** - Buy menu configuration file

## 🚀 Usage

### Installation

1. Clone or download this repository
2. Copy all `.cfg` files to CS2 config directory:
   ```
   Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\
   ```
3. Add Steam launch options:
   - Right-click CS2 in Steam library → Properties → General → Launch Options
   - Add the following launch options:
     ```
     -high -tickrate 128 -allow_third_party_software +exec autoexec.cfg
     ```
   - `-high` - Sets process priority to high
   - `-tickrate 128` - Sets tickrate to 128 (for local servers)
   - `-allow_third_party_software` - Allows third-party software
   - `+exec autoexec.cfg` - Executes autoexec.cfg on launch

### Main Config Features

- **Sensitivity**: 1.76
- **Crosshair**: Purple crosshair, small size
- **Viewmodel**: FOV 68, custom offsets
- **Key Bindings**: 
  - `Left Alt` - Switch hands (left/right hand toggle)
  - `C` - Flashbang quick switch
  - `N` - Jump throw bind
  - `B` - Radar scale toggle
  - `7` - Switch to online config (for community servers)
  - `Mouse5` - Rethrow last grenade (practice mode)
  - `M` - Timescale toggle (practice mode)
  - `Y` - Place bot (practice mode)

## ⚙️ Customization

Modify the following files according to your preferences:
- `x.cfg` - Main game settings
- `autoexec.cfg` - Commands executed on startup
- `buy.cfg` - Buy menu settings

## 📝 Notes

- Some binds (like `sv_rethrow_last_grenade`) only work with `sv_cheats 1`
- Config files are compatible with both CS:GO and CS2
- Press `7` to switch to `x_online.cfg` when playing on community servers (removes buy commands that may be restricted)
- It's recommended to backup your original config before modifying