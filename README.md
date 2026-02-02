# 🎮 Ayaneo Pocket Air Mini: Zero to Hero Setup Guide

Welcome to the ultimate guide for transforming your Ayaneo Pocket Air Mini (PAM) into a high-performance retro gaming powerhouse. This guide covers everything from the initial unboxing to "Dark Arts" system optimizations.

---

### ☕ Support My Work
If this guide saves you hours of frustration and helps you build your dream handheld, consider buying me a coffee!

<a href="https://www.buymeacoffee.com/hackerman_0" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

---

## 🛠️ Phase 1: Preparation & Materials

Before we begin, ensure you have the following ready:
* **The Device:** Ayaneo Pocket Air Mini (charged to at least 60%).
* **Storage:** A high-quality MicroSD card (128GB to 512GB+ recommended).
* **Software:** Download these apps from the Play Store or their official sites:
  * **Frontend:** ES-DE (EmulationStation Desktop Edition)
  * **File Managers:** MiXplorer or ZArchiver
  * **Torrent Manager:** Flud
  * **Editors:** QuickEdit
  * **System Tools:** AccuBattery, Shizuku, Termux
  * **Emulators:** RetroArch, Dolphin, NetherSX2, PPSSPP, Duckstation, Azahar, MelonDS, Mupen64Plus FZ.

---

## 🍳 Phase 2: Mixing the Ingredients (The Recipe for Success)

### **1. System & Firmware Updates**
Ensure the "brain" of your device is up to date.
1. Open the **System Update** app. Install all updates and **Restart**.
2. Open the **Ayasettings** app. Perform the internal update and **Restart** again.

### **2. Virtual Memory Booster**
Crucial for heavy systems like PS2 or Switch:
1. Open **Ayasettings**.
2. Go to **Device -> Virtual Memory Management**.
3. Set the value to **3GB** and enable the **Swap** switch below it.

### **3. Setting up Flud (The Download Manager)**
1. Open **Flud** and grant permissions.
2. Tap the Menu (top left) -> Select **SD Card**.
3. Navigate to the `Downloads` folder.
4. Tap the **"+" folder icon** (top right), name it `Flud`, and select **"Use this folder"**.

---

## 📂 Phase 3: Finding Your Library (The Directions)

I cannot provide direct links, but I can show you the way.

* **The Starter Pack:** Search Google for **"tiny best set: go! archive"**.
  * Look for the **94 GB** version.
  * Download the **Torrent file** from the bottom of the page and open it with Flud.
* **The Holy Grail:** Remember the keyword **"Megathread"**. It is the paradise for retro gamers looking for specific console ROMs and BIOS files.

---

## 🎨 Phase 4: ES-DE Initial Setup & Folders

1. Open **ES-DE**.
2. **Data Directory:** Select your **SD Card** -> Create folder `ES-DE` -> Select **"Use this folder"**.
3. **ROMs Directory:** Select your **SD Card** -> Create folder `ROMS` -> Select **"Use this folder"**.
4. Tap **"Create them"**, then **"I understand"**. Once finished, **fully close** the app.

### **Organizing BIOS & ROMs**
Using **ZArchiver**, navigate to your downloaded `tiny set best go-games`:
1. **BIOS:** Copy everything from the `bios` folder and the `expansion-64` folder inside the zip to the `BIOS` folder on your **SD Card**.
2. **ROMs:** Move game files into their corresponding folders inside the `ROMS` directory on your SD card. 
3. **Pro Tip:** Delete the zip files after extraction to save space!
## ⚙️ Phase 5: Emulator Configuration (The Pro Setup)

### **1. RetroArch (Multi-System Hub)**
Open RetroArch and grant permissions.
* **Visuals:** Settings > User Interface > On-Screen Notifications > Scale Graphics Widgets Automatically: **OFF** | Graphics Widgets Scale Override: **0.75x**.
* **Controls:** Settings > Input > Retropad Binds > Port 1 > Analog to Digital Type: **Left Analog**.
* **Hotkeys (L3 as Enable Button):**
    * Menu Toggle: **L3 + R3** | Quit: **Start + L1** | Fast Forward: **R2** | Slow Motion: **L2**.
    * **Save State: R1** | **Load State: L1** | Screenshots: **Y**.
* **Directories:** Settings > Directory. Point **System/BIOS**, **Saves**, and **Save States** to their respective folders on your **SD Card**.
* **Speed Hack:** Open `Android/data/com.retroarch.aarch64/files/retroarch.cfg` with **QuickEdit**. Add `input_threaded = "false"` at the bottom.
* **Shaders:** Use `LCD-Grid-V2` for Handhelds and `CRT-Lottes` for TV consoles. Avoid "Mega Bezel".

### **2. Dolphin (GameCube & Wii)**
* **Paths:** Add `SD Card > ROMS > GC` and `Wii` folders.
* **Graphics:** Video Backend: **Vulkan** | Shader Compilation: **Skip Drawing** | Compile Shaders Before Starting: **ON**.
* **Resolution:** Internal Resolution: **2x Native**.
* **Performance:** Config > Advanced > Emulated CPU Clock Speed: **60%-70%**.
* **Wii Controls (FPS Setup):** Extension: **Classic**. Map ZL/ZR to L1/R1 and Triggers to L2/R2.

### **3. NetherSX2 (PlayStation 2)**
* **BIOS:** Import from `SD Card > BIOS`.
* **Graphics:** Renderer: **Vulkan** (or OpenGL if Vulkan glitches) | Threaded Presentation: **ON**.
* **Underclocking (Crucial):** Settings > System > EE Cycle Rate: **75%** | EE Cycle Skip: **1** | Multi-threaded VU1: **ON**.
* **Controls:** Controller Port 1 > Automatic Mapping.

### **4. PPSSPP (PSP)**
* **Graphics:** Backend: **Vulkan** | Rendering Resolution: **2x** | Frame Skipping: **1** | Auto Frameskip: **ON**.
* **Performance:** Lazy Texture Caching: **ON** | Fast Memory: **OFF** | Ignore Bad Memory Accesses: **ON**.

### **5. Duckstation (PS1)**
* **Graphics:** Renderer: **Vulkan** | Resolution Scale: **3x or 4x** | PGXP Operation Mode: **Memory Only** (fixes wobbly textures).
* **Controller:** Set Touchscreen View to **None**.

### **6. Azahar (3DS)**
* **Graphics:** API: **Vulkan** | Resolution: **3x**.
* **Mapping:** Screen Swap: **L3** | Cycle Layout: **R3**.

### **7. MelonDS (DS) & Mupen64Plus FZ (N64)**
* **MelonDS:** Set Resolution to **2x/3x**. Map Screen Swap to **L3**.
* **Mupen64Plus FZ:** Use **GLideN64-Very-Accurate** profile. Map **C-Buttons** to the **Right Analog Stick**.
## 🎨 Phase 6: ES-DE Advanced Setup & Scraping

Make your collection look professional and set ES-DE as your permanent home.

1. **Interface:** Start Menu > UI Settings > Theme Downloader. Download **"Art Book Next"**.
2. **Scraper (Game Art):**
   * Register for free at [screenscraper.fr](https://www.screenscraper.fr/).
   * Enter credentials in **Scraper > Account Settings**.
   * Select your desired metadata (Box art, screenshots, etc.).
   * Set **Region** and **Language**.
   * **Start Scraping:** This may take several hours. It is recommended to run this overnight.
3. **App Integration:** * Utilities > Game Importer > Import to System: **Android Apps**.
   * Select your installed apps (Flud, Chrome, etc.) and Import.
   * Repeat for **Emulators** to have quick access to standalone apps.
4. **Default Launcher:** * Android Settings > Apps & Notifications > Default Apps > Home App.
   * Select **ES-DE**.

---

## ⚡ Phase 7: System Optimization & Battery Health

### **1. Developer Performance Tweaks**
Go to **Settings > System > Developer Options**:
* **Window/Transition/Animator Scale:** Set all to **0x (Off)**.
* **Background Process Limit:** Set to **2**.
* **Disable HW Overlays:** **ON**.
* **Force GPU Rendering:** **ON**.

### **2. Battery Health (AccuBattery)**
1. Open **AccuBattery**.
2. Set the **Charge Alarm to 80%**.
3. Always unplug at 80% to maximize the lifespan of your PAM's internal battery.

---

## 🌑 Phase 8: The Dark Arts (Advanced Debloating)

Free up RAM and CPU cycles by disabling hidden background services using **Shizuku** and **Termux**.

1. **Shizuku:** Start via **Wireless Debugging**. Export files to `SD Card/Ter`.
2. **Rish Script:** Open `SD Card/Ter/rish` with **QuickEdit**. 
   * On **Line 24**, change the PKG value to: `"com.termux"`.
3. **Termux execution:**
   * Open Termux. Type: `cd /storage`, then `ls` to find your SD ID (e.g., `0123-4567`).
   * Type: `cd /storage/YOUR-ID-HERE/Ter`.
   * Type: `sh rish` and press Enter.
   * **Paste the following commands:**

```bash
pm disable-user --user 0 com.android.dreams.basic
pm disable-user --user 0 com.android.egg
pm disable-user --user 0 com.android.wallpaper.livepicker
pm disable-user --user 0 com.android.wallpaperbackup
pm disable-user --user 0 com.android.traceur
pm disable-user --user 0 com.google.android.feedback
pm disable-user --user 0 com.google.android.printservice.recommendation
pm disable-user --user 0 com.google.android.onetimeinitializer
pm disable-user --user 0 com.google.android.apps.restore
pm disable-user --user 0 com.google.android.ims
pm disable-user --user 0 com.mediatek.engineermode
pm disable-user --user 0 com.mediatek.mtklogger
pm disable-user --user 0 com.mediatek.gnssdebugreport
pm disable-user --user 0 com.mediatek.batterywarning ```
4. **Restart your device.** Your PAM is now cleaner and faster than ever!

---

### ☕ Final Support
If this "Zero to Hero" guide helped you build the perfect handheld, consider supporting my work!

<a href="https://www.buymeacoffee.com/hackerman_0" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

**Happy Gaming!** 🕹️✨
