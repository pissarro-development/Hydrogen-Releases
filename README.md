# Kernel flash guide for Redmi Note 11 Pro+ 5G (pissarro*)

## Prerequisites

1. Unlocked bootloader
2. Installed platform tools (adb) on your computer
3. Installed custom recovery (AOSP / TWRP / OrangeFox and etc.)

## Flashing Instructions

### 1. Boot into Recovery mode

- Power off your device.
- Hold the appropriate key combination (typically **Volume Up + Power**) to enter Recovery mode.

### 2. Flash Kernel ZIP

In the recovery menu:

- Select **Install**
- Navigate to the AnyKernel3 kernel `.zip` file  
  *(or push it first via ADB sideload — see below)*

**Option A — flash from internal storage:**  
Copy the kernel ZIP to your device beforehand, then select it in the Install menu.

**Option B — ADB sideload:**  
In the recovery menu select **Apply update → Apply from ADB**, then on your computer run:
```bash
adb sideload <kernel-zip-name>.zip
```
### 3. Confirm instalaltion

Swipe or enter power button to confirm the flash.

### 4. Reboot to System

After the flash completes, return to the main recovery menu and select **Reboot → System**.

### 5. Done

Your device will boot with the new kernel. First boot may take slightly longer than usual.
