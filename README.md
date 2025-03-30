# GTA Online Apartments Trade-In Exploit Script

This is an automated script (AHK, v1.1 for now) for using the apartments trade-in exploit in GTA Online.

---

## Table of Contents
1. [WARNING](#warning)
2. [Requirements](#requirements)
3. [Installation](#installation)
4. [IMPORTANT](#important)
5. [Controls](#controls)
6. [NOTES](#notes)
7. [Known Bugs](#known-bugs)
8. [Planned Improvements](#planned-improvements)

---

## WARNING
I take **no responsibility** for any bans, suspensions, or other consequences resulting from the use of this script.  
Every user applies this script **at their own risk**.

---

## Requirements
For this to work, you need:
1. **GTA5 E&E (Enhanced & Expanded)** version of the game (ATM it **DOESN'T WORK** on Legacy Edition),
2. Game set to `1024x768` windowed mode,
3. Game's language set to **English**,
4. Safezone size set to **7 ticks**:
   - Go to `Settings > Display`, set it to max (all the way to the right), then tap left three times,
5. Phone alerts set to **OFF** and Message Frequency set to **1 hour**:
   - Go to `Settings > Notifications`,
6. Frame Limit set to **60 fps** and Pause Game on Focus Loss set to **OFF**:
   - Go to `Settings > Graphics`,
7. "Snapmatic Quick Launch" set to **OFF**:
   - Pull up the phone while in GTA Online, press the right arrow until you reach the "settings" tile, enter it, then go to "Snapmatic" and choose "Snapmatic Quick Launch OFF",
8. Spawn Location set to any building **except**:
   - Apartments, Garages, or entity-packed locations like LS Car Meet (examples: Hangar, Facility, Kosatka, Auto Shop).

---

## Installation
1. Download the [`.zip`](https://github.com/tetriskillerh/gtaoautoapps-Fix/releases/latest) file and extract it (you need to install AutoHotKey v1.1 to use the script),  
   or  
2. Download the [`.exe`](https://github.com/tetriskillerh/gtaoautoapps-Fix/releases/latest) file (no installation required, but you cannot customize the hotkeys in the .exe version).

---

## IMPORTANT
The script will ask for **admin rights**.  
It won't run without admin rights because it needs them to add and remove firewall rules used for NoSave. Without admin rights, NoSave will not work.

---

## Controls
### **Numpad0**: Start Preparation Phase  
- Sets up all 10 slots to a value of `$550k` each.  
- This must be run in **Story Mode**. Start the process and wait until it completes.

### **Numpad1**: Start Payback Phase  
- This is the **main hotkey** used for "selling apartments" after all slots are prepared.  
- This must be run in **Story Mode**. An input box will appear where you can specify the number of runs. Start the process and wait until it completes.

### **Numpad2**: Enable No-Save Mode ("panic button")  
- Manually enables No-Save Mode, preventing the game from saving progress.

### **Numpad3**: Disable No-Save Mode ("panic button")  
- Manually disables No-Save Mode, allowing the game to save progress again.

### **Numpad4**: Reload Script ("panic button")  
- Reloads or resets the entire AHK script.

### **Numpad5**: Exit Script ("panic button")  
- Completely terminates the script and disables No-Save Mode if it is active.

### **Numpad6**: Cycle Slow Mode  
- This hotkey cycles through different delay options for Slow Mode.  
- The delay cycles through `0ms`, `50ms`, `100ms`, ..., up to `300ms`.  
- Use this if the script frequently fails during tasks like selecting apartments or navigating the web browser, such as accidentally opening Legendary Motorsport instead.  
- **Tip:** Holding `Numpad6` for more than 500ms will immediately reset the delay to `0ms`, without needing to cycle through all options.
- **Default:** `0ms` (disabled).

### **Numpad9**: Toggle NoSave Status Display  
- Toggles the display of the NoSave status.  
- When enabled, a tooltip will show whether NoSave Mode is active or inactive.
- Use this to visually monitor the NoSave state.
- Hold `Numpad9` to activate debugging tooltips for better troubleshooting. 
- **Default:** `off`.

---

## NOTES
- Feel free to change hotkeys to your own preferences (if using the `.ahk` version).  
- If you encounter issues, ensure all requirements are met and admin rights are granted.  
- Before creating a new issue, please check the [Known Bugs](#known-bugs) section to see if the problem is already documented.

---

## Known Bugs
- ([#6](https://github.com/tetriskillerh/gtaoautoapps-Fix/issues/6)) ???it may be broken at this time test it and if it is make a bug report???
- ([#7](https://github.com/tetriskillerh/gtaoautoapps-Fix/issues/7)) R Menu Still bug's out the Script.

---

## Planned Improvements
- **Customizable Hotkeys in `.exe` Version:** Add support for changing hotkeys directly in the `.exe` version.
- **Enhanced Debug Mode:** Provide more detailed logs for troubleshooting.
- **Multi-Language Support for Script Menus:** Allow users to choose the language for script popups and menus (e.g., the prompt asking for the number of runs).
