# 20260311
- QPR2 release
- ship with 4.19.325-cip128-st12 kernel
- updated statusbar padding and height

# 20260116
- **Happy new year.**
- **Now ships with non KSU version of Cirno kernel by default + cip126 merged**
- Sync to PixelOS-AOSP sixteen-qpr1 latest sources
- Fix lock icon being too small in lock screen
- Fix DND icon in new reverse-engineered smartspace

# 20251221
- Android 16 QPR1 build + Material 3 Expressive
- [enable lockscreen landscape mode](https://review.lineageos.org/c/LineageOS/android_frameworks_base/+/465790) - this also enable new landscape mode QS (not a split shade hack through device overlay)
- update statusbar paddings and fix round corners drawables not rendered properly on "Hide" display cutout
- ship with 4.19.325-Cirno kernel (KSU)

# 20251103
- Sync sources
- Updated prebuilt kernel

# 20251101-a
- [Fix default lockscreen clock font](https://github.com/pos-fog/android_vendor_lineage/commit/dc948aa074e19e7c4a666efc3cc835f9489ccf00)
- [config: enable OTA updater for unofficial builds](https://github.com/pos-fog/android_vendor_custom/commit/968f34208e44e773d8b11fe98e5938d3e721d748)
- Hide procfs related audit messages from appdomain

# 20251101
> NOTE: dirty flashing from 20250727 build is not recommended due to regenerated signing keys and user build
- New build with new sources from PixelOS-AOSP + personal changes
- Switch to user build
- Ship with new prebuilt kernel, with KernelSU built-in and bpf 5.10 backports
  #### Device tree changes:
  - sync to `lineage-23` branch
  - Revert "fog: props: Move input surface to CCodec" (causes screen record (and possibly video recording) lagging due to use of c2 swcodec as input source instead of OMX hwcodec)
  - fog: props: Make SurfaceFlinger latch all buffers unsignaled

# 20252707
- Updated prebuilt kernel
- For new installation (clean flash), I no longer shipped Gmail and Google Maps
- Some minor source changes

# 20252007
- Settings: Remove "Google Play System Update" in Android Version
- Properly disable some unused GMS components and disable Pixel Battery widget
- Some minor misc. changes

# 20251807
- Drop reverse-engineered Google Pixel smartspace (At A Glance) implementation on SystemUI due to brokenness on BP2A/Android 16

# 20251707
- Fix Circle to Search not working
- Added new bootanimation for 720p display

# 20251607
- Initial Android 16 build
