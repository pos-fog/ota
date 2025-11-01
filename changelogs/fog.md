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
