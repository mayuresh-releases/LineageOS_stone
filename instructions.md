# LineageOS for Redmi Note 12 5G / POCO X5 (stone)

# 📲 Installation Instructions

---

## ⚠️ Before You Begin

- Backup **all important data** to an external source. This process will erase your internal storage.
- A **clean flash** is mandatory if you're switching from another ROM.
- You **must be on the latest firmware** available for your device and region. Flash it manually if needed before proceeding.
- **Recommended Recovery:** Use **AOSP recovery**.

---

## 🧹 Clean Flash (Recommended for First-Time Install)

1. **Boot into Fastboot mode**
   - Power off your device and use the hardware button combo
   **OR**
   - Run:
     ```bash
     adb reboot bootloader
     ```

2. **Flash the recovery image**
   ```bash
   fastboot flash boot boot.img
   ```

3. **Reboot into Recovery**
   ```bash
   fastboot reboot recovery
   ```

4. **Format data**
   - In recovery:
     `Factory Reset > Format Data`

5. **Connect the phone to your PC**

6. **Sideload the ROM**
   - In recovery:
     `Apply update > Apply from ADB`
   - On your PC, run:
     ```bash
     adb sideload lineage-23.2-xxxx-UNOFFICIAL-stone.zip
     ```

7. **(Optional)** When prompted after sideloading, choose **Yes** to reboot to recovery again if you want to flash:
   - GApps
   - Magisk
   - Any other additional `.zip`

8. **Format data again** if you flashed anything in Step 7

9. If you're not flashing anything else, choose **No** when prompted

10. **Reboot to system**
    *(Note: First boot may take several minutes)*

---

## 🔄 ROM Update / Dirty Flash (For Updating Same ROM)

You can update your ROM using one of the following methods:

---

### ✅ Option 1: OTA Update
- Go to:
  `Settings > System > Updater`
- Download and install the new build
- Click reboot
- Done!

---

### ✅ Option 2: Local Update (Via Updater App)
1. Place the new ROM `.zip` on your internal storage
2. Open the **Updater app**
3. Tap the 3-dot menu > **Local Update**
4. Select the ROM `.zip` and confirm
5. The update will install seamlessly in the background.
6. Tap **Reboot** when the installation completes.

---

### ✅ Option 3: Manual Dirty Flash (ADB Sideload)

1. **Boot into Recovery**

2. In recovery:
   `Apply update > Apply from ADB`

3. On PC, sideload the ROM:
   ```bash
   adb sideload lineage-23.2-xxxx-UNOFFICIAL-stone.zip
   ```

4. **(Optional)** Reboot back to recovery and sideload any additional zips you had earlier:
   - GApps
   - Magisk

5. **Reboot to system**

---

## ✅ You're Done!
Enjoy your freshly installed or updated ROM.
