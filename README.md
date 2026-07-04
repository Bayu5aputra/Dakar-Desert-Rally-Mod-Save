<div align="center">
  <h1>🏜️ Dakar Desert Rally - Save Editor & DLC Unlocker</h1>
  <p>A simple web-based tool to modify player stats and unlock DLCs directly via binary GVAS save files.</p>
  
  <br />
  <a href="https://github.com/Bayu5aputra/Dakar-Desert-Rally-Mod-Save/releases/latest">
    <img src="https://img.shields.io/github/v/release/Bayu5aputra/Dakar-Desert-Rally-Mod-Save?style=for-the-badge&color=success&label=DOWNLOAD%20LATEST%20RELEASE" alt="Download Release" />
  </a>
  <br />
</div>

---

## 🌟 Features

- **Modify Player Stats**: Change your Player Level (up to 999), Dakar Points (Money), and Total Experience Points.
- **DLC Unlocker**: Seamlessly inject unlocked DLC data directly into your save file.
- **Stage Skipper (Beta)**: Instantly transfer all completed events/stages from a 100% save file into your own save file.
- **100% Local & Safe**: No software installation required. Runs entirely locally in your web browser (Client-side only, no data is uploaded to any server).
- **Epic Games Store Support**: Includes **ScreamAPI** to bypass DLC entitlement checks for EGS players.

## 📂 Repository Contents

- `index.html` - The main Web-based Save Editor application.
- `stage_skipper.html` - The Beta tool used to transfer 100% progression between save files.
- `ScreamAPI-v4.0.0/` & `.zip` - The tool required to unlock DLCs (for Epic Games Store users).
- `DakarDRSave2Slot_...sav` - A backup/example save file.

---

## 🚀 How to Use the Save Editor

### 1. Locate your Save File
Find your Dakar Desert Rally save file on your PC. It is typically located at:
```text
%LOCALAPPDATA%\Dakar2Game\Saved\SaveGames\
```
*(Tip: Press `Win + R`, paste the path above, and hit Enter)*

### 2. Open the Editor
Double-click `index.html` to open it in any modern web browser (Chrome, Firefox, Edge, Safari, etc.). 

### 3. Edit Your Save
- **Drag and Drop** your `.sav` file into the designated drop zone in the browser.
- Modify the values as you see fit: **Player Level**, **Dakar Points**, and **Total Experience Points**.
- Select the DLCs you wish to unlock under the **Unlock DLCs** section.

### 4. Save and Apply
- Click the **"Save Changes & Download .SAV"** button.
- **⚠️ Important:** Make a backup of your original `.sav` file before overwriting!
- Replace your original save file in the `SaveGames` folder with the newly downloaded `.sav` file.

---

## ⏭️ How to Use the Stage Skipper (Beta)

If you want to skip the grind and instantly unlock all stages, you can use the new Stage Skipper tool to merge a 100% completed save into your own.

### 1. Requirements
- Your current 0% (or partially completed) save file (`DakarDRSaveSlot.sav`).
- A 100% completed save file downloaded from the internet.

### 2. Open the Skipper
- Double-click `stage_skipper.html` to open it in your browser.

### 3. Transfer Progression
- Click the **Target Save** box and upload your personal save file.
- Click the **Source 100% Save** box and upload the 100% completed save file.
- Click **"Transfer 100% Stages"**.
- A new file named `DakarDRSaveSlot_100Percent.sav` will be downloaded. Rename this to match your slot (e.g., `DakarDRSave1Slot.sav`) and place it in your `SaveGames` folder.

---

## 🔓 How to Use ScreamAPI (Epic Games Store)

If you play the game on the **Epic Games Store** and unlocked DLCs in the save editor, you **MUST** install ScreamAPI so the game properly reads and authorizes those DLCs.

1. Navigate to your game's installation directory, specifically the `Win64` binaries folder:
   ```text
   [Your Game Install Folder]\Dakar2Game\Binaries\Win64\
   ```
2. Locate the file named `EOSSDK-Win64-Shipping.dll`.
3. **Rename** the original `EOSSDK-Win64-Shipping.dll` to `EOSSDK-Win64-Shipping_o.dll` (this acts as your safe backup).
4. Open the `ScreamAPI-v4.0.0` folder included in this repository.
5. Copy the `ScreamAPI64.dll` file.
6. Paste it into the `Win64` folder of your game (where you just renamed the original file).
7. **Rename** the copied `ScreamAPI64.dll` to `EOSSDK-Win64-Shipping.dll`.

> **Note**: Do not use the `ScreamAPI.config.json` file unless you are troubleshooting, as its default logging feature can negatively impact game performance.

---

## ⚠️ Disclaimer
Use this mod at your own risk. Modifying save files can sometimes lead to unexpected behaviors or corruption. **Always back up your save files before making any modifications.**
