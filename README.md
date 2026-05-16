# 📱 Termux ROM Flasher

Flash Fastboot ROMs directly from one Android phone to another using Termux.

---

## 🚀 Getting Started & Installation

Follow these steps carefully to set up your environment and flash your ROM.

### Step 1: Install Termux & Termux:API
* 📥 **Download:** [Termux App (Latest)](https://github.com/termux/termux-app/releases/latest)
* 📥 **Download:** [Termux:API App (Latest)](https://github.com/termux/termux-api/releases/latest)

### Step 2: Set Permissions (Termux:API App)
After installing both apps, configure your device settings to prevent background termination:

1. Open the **Termux:API** app.
2. Grant **Draw over other apps / Display pop-up windows**.
3. Set **Battery Saver** to **No restrictions**.
4. **China ROM only:** Set **Get info about all apps** to **Always allow**.

### Step 3: Grant Storage Access
Open Termux and run:
```bash
termux-setup-storage
```
### Step 4: Install MiTool [(Credit)](https://github.com/offici5l/MiTool)
Run this command in Termux:
```bash
curl -sS https://raw.githubusercontent.com/offici5l/MiTool/master/install.sh | bash
```
Accept any permission popups that appear in Termux during setup.
### Step 5: Extract the ROM
Extract your target Fastboot ROM zip file into your device's internal storage using any file manager.
### Step 6: Navigate to the ROM Folder
Use the `cd` command to enter the directory where you extracted the ROM.

```bash
cd /storage/emulated/0/"path to your folder"
```
*Example :*
```bash
cd /storage/emulated/0/HyperOS.Turbo-OS3.0.7.0.VNQCNXM-Gold.Iron/
```
### Step 7: Execute the Flash Script
1. Reboot your target smartphone into **Fastboot Mode** and connect it to your flashing device.
2. Run the installer script using:
```bash
bash flash_all.sh
```
A Termux:API popup will appear on your screen. Make sure to allow the permission immediately, and your flashing will start.
### ⏳ What to Expect Next
* The flashing process will begin in the terminal output. **Do not disconnect the cable.**
* The process takes several minutes. Sit back and wait.
* Once the flashing successfully completes, your target device will **automatically reboot** into the system.

**🎉 Enjoy your new ROM!**

