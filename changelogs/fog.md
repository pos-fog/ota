# June 8, 2025
- **Do not install this OTA on 20 May build since signing keys are re-generated. This is for 6 June build users**
- **June 2025 security patch**
- **fixed kernel issue that caused to stuck at Mi logo when rebooting to recovery**
- powerhint: Bring back CPUBigClusterMinFreq on INTERACTION

# June 6, 2025
- **Maybe the last before Android 16**
- **this build is not rolled out to OTA updates, you need to manual flash due to re-generated signing keys**
- Remove some deprecated stuff on overlays
- Update `surfaceflinger` durations
- Completely disable attestation hooks by default (to pass Integrity, use PIFork and TrickyStore with Tricky Addon + valid keyboxes or 'use AOSP keybox')
- Bring back Android Go configurations
- Revert split shade QS (as per feedback)
- init: add context_hub into audio hal group
- init: Add "system" group to Audio HAL
- Silence HWUI Logspam
- Update `powerhint.json` - remove non-existing nodes due to kernel change, and reducing log spam
- and misc. things

# May 20, 2025
- Introduce **DeviceAsWebcam**
- Drop `ro.surface_flinger.force_hwc_copy_for_virtual_displays` prop

# May 16, 2025
- Default DPI now set to 280 (411 dp)
- Add Google Recorder app by default
- Drop legacy `armeabi` support (doesn't affect anything except if you uses legacy Android applications that targetted for Android version older than Marshmallow/Nougat)
- Build QTI USB Gadget HAL
- Switch to NCM USB Tethering
- and misc. changes

# May 1, 2025
- props: Import lmkd props from rhode (NOTE: I use Simple LMK on prebuilt kernel, but it's nice to have it for preserving compatibility with custom kernel that uses userspace LMK/LMKD)
- overlay: Enable split shade QS on landscape mode
- Sync sources to PixelOS-AOSP latest commits

# April 25, 2025
- Replace Accord with Gramophone music player by default
- Updated prebuilt kernel (update defconfig - now CPU freq governor defaults to `schedutil`)
- Sync with latest PixelOS sources

# April 19, 2025
- April secpatch
- powerhint: Restrict max CPU freq to critical hints
- init: Align cpusets with crosshatch
- Revert "fog: rootdir: Start bootanimation on post-fs"
- Drop MIUI offline charging (chargeonlymode)
- Switch to AOSP offline charging animation

# April 1, 2025
- Sync sources

# March 28, 2025 (revision 3)
- Add Accord music player
- Replace Aperture with GrapheneOS Camera

# March 28, 2025 (revision 2)
- Fix GameSpace is not installed

# March 28, 2025
- March 2025 (QPR2) update
- Switch to my custom fork of PixelOS
- Add GameSpace (from Pixelage)
- Add GamesPropsHooks to unlock FPS or high graphic settings in some games
- Add app cloning support
- Switch to common Lights HAL
- Disable GMS Key Attestation block by default (allow compatibility with PIF/Tricky Store module)
- Switch to Pixel power-libperfmgr
