# Home Route – Downloads

Drive and walk through real places, built on your PC from open map data.

**[➜ Download the latest version](https://github.com/mimiundmomotv-wq/HomeRoute-Releases/releases/latest)**

## Installation, step by step

### What you need
- A **Linux** PC (64-bit) with **Ubuntu 24.04** or newer, Debian 13, Fedora 39 or newer, or another current distribution. Windows and Mac are not supported yet.
- A graphics card with a current driver (Vulkan). AMD and Intel graphics usually work out of the box on Ubuntu, Fedora etc. For NVIDIA, install the NVIDIA driver (Ubuntu: *Software & Updates → Additional Drivers*).
- At least 16 GB of RAM, about 1 GB of free disk space for the game, plus a few GB for each area you build.
- An internet connection for building new areas.

### 1. Download
1. Open the **[latest version](https://github.com/mimiundmomotv-wq/HomeRoute-Releases/releases/latest)** page.
2. Scroll down to **Assets**.
3. Click **`HomeRoute-…-Linux-x86_64.tar.gz`** (the big file, a few hundred MB).
   You do **not** need "Source code (zip)" or "Source code (tar.gz)": GitHub adds them automatically and they only contain this guide.
4. The file usually ends up in your **Downloads** folder.

### 2. Unpack
1. Open **Downloads** in your file manager.
2. Right-click `HomeRoute-…-Linux-x86_64.tar.gz` → **"Extract here"**.
3. You get a folder `HomeRoute-…-Linux-x86_64`. Move it wherever you like; you can delete the `.tar.gz` afterwards.

### 3. Start
1. Open the unpacked folder.
2. Double-click **`HomeRoute.sh`**.
   - **KDE (Dolphin):** if asked, choose **"Execute"**.
   - **GNOME/Ubuntu (Files):** if a text editor opens instead, close it, right-click `HomeRoute.sh` → **"Run as a Program"**.
   - **If that doesn't work**, use a terminal: right-click inside the folder → "Open in Terminal", type this and press Enter:
     ```
     ./HomeRoute.sh
     ```
3. The first start takes a little longer (up to a minute) while the graphics are prepared.

### 4. Play
- **First time:** "Choose area" → "Starter Town" → **"Drive"**: a made-up village, playable at once.
- **Build your own place:** "New area" → type a town or street → "Search" → click a result → choose the size → **"Create area"**. The data is downloaded and built, which takes a few minutes depending on the size. Works best in **North Rhine-Westphalia** (Germany); other German states as far as they publish open 3D building data.
- **Choppy?** Choose **Low** in "Settings".

**Keys**

| Key | What it does |
|---|---|
| W / S | Accelerate / brake (on foot: forward / back) |
| A / D | Steer (on foot: sideways) |
| Space | Handbrake (on foot: jump) |
| Mouse | Look around |
| F | Get out / get in |
| C | Call the car to you |
| R | Reset the car |
| H | Back to the start |
| Tab | Map: click a place or search a street to jump there |
| V | Fly (F lands you on foot again) |
| M | Mark a spot with a comment (for bug reports) |
| Esc | Menu |

### Your data, uninstalling, updating
- Your areas and settings are in `~/.config/Epic/HomeRoute/` (a hidden folder in your home folder; **Ctrl+H** shows hidden files).
- **Uninstall:** delete the `HomeRoute-…-Linux-x86_64` folder, and `~/.config/Epic/HomeRoute/` too if you want your areas and settings gone.
- **Update:** download and unpack the new version; your areas are kept.

### If something goes wrong
- **Doesn't start / black screen:** update your graphics driver; start it from a terminal (`./HomeRoute.sh`) to see the error.
- **"Create area" stops right away:** check your internet connection.
- **Report a problem:** click **Issues → New issue** at the top of this page and describe what happened (a screenshot helps).

*Checksum (optional):* put the `.sha256` file next to the archive and run `sha256sum -c HomeRoute-*.tar.gz.sha256`; it should print "OK".

---
Licences: game code MIT, own assets CC BY-SA 4.0 / CC0. Map data © OpenStreetMap contributors (ODbL); geodata of the German states under their open licences (see Credits in the game). Built with Unreal Engine. This repository only holds the downloads.
