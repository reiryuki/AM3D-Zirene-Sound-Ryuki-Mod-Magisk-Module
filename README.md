# AM3D Zirene Sound Ryuki Mod Magisk Module

## DISCLAIMER
- AM3D apps and blobs are owned by AM3D™.
- The MIT license specified here is for the Magisk Module only, not for AM3D apps and blobs.

## Descriptions
- Equalizer sound effect ported from SHARP Aquos SHV33 and integrated as a Magisk Module for all supported and rooted devices with Magisk
- Global type sound effect

## Sources
- KDDI/SHV33_jp_kdi/SHV33:7.0/SB201/03.02.09:user/release-keys
- AM3DZireneSound.apk: https://github.com/therealahrion/AM3D-Zirene-Sound
- libam3daudioenhancement.so: https://forum.xda-developers.com/t/am3d-zirene-reg-sound-unity-deprecated.3396698/page-37 AM3D_Nougat_libraries.zip
- libmagiskpolicy.so: Magisk (stable) 30.7 (30700)

## Screenshots
https://t.me/androidryukimodsdiscussions/26291

## Changelog

v3.3
- Support NoMount metamodule
- Update libmagiskpolicy.so from Magisk (stable) 30.7 (30700)
- Move _uninstall.log to /data/adb/logs/

v3.2
- Does not disable raw playback (You can use Audio Compatibility Patch Reborn Magisk Module instead)

v3.1
- Fix wrong target in latest KernelSU

v3.0
- Tidy up aml.sh
- Exclude \*audio\*effects\*haptic\*.xml
- Abort installation if fail to mount mirror system
- Fix wrong file permissions in some ROMs

v2.19
- Improve /odm and /my_product support detection

v2.18
- Add Action button to clear apps caches
- Fix architecture detection in some weird ROMs
- Apply effect to rerouting and patch stream by default for game apps
- Fix bug in uninstall.sh

v2.17
- Allow installation in Android Emulator

v2.16
- Improve audio_effects.xml patch detection
- Fix conflict with modules_update while installing via recovery if Magisk installed
- New Magisk and Kitsune Mask support (independent mirror)
- Remount partitions before mounting mirror to prevent mount failure caused by device/resource busy
- Prevent double chain while using post process music stream with ro.am3d.music_stream boolean parameter
- Fix MagiskHide & SUList
- Fix script bug
- Update sepolicy rules

v2.15
- Fix script bug
- Redirect /sdcard to /data/media/"$UID"
- Sets system property ro.audio.monitorWindowRotation=true if audio.rotation=1 at optionals.prop
- Fix MagiskHide & SUList
- Kitsune Mask detection

v2.14
- Specify UID at script
- Add optional debug.log=1 for more detailed install log
- Support 64 bit only ROM
- Fix mount partitions
- Sets ro.audio.ignore_effects to false

## Requirements
- arm64-v8a or armeabi-v7a architecture
- Android 4.4 (SDK 19) until 8.1 (SDK 27) only
- HIDL audio service
- Magisk or Kitsune Mask or KernelSU or Apatch installed

## Installation Guide & Download Link
- If you are using KernelSU, you need to disable Unmount Modules by Default in KernelSU app settings and install https://github.com/KernelSU-Modules-Repo/meta-overlayfs or https://github.com/KernelSU-Modules-Repo/magic_mount_rs or https://github.com/KernelSU-Modules-Repo/hybrid_mount or https://github.com/maxsteeel/nomount first depending on ROM compatibility
- Install this module https://devuploads.com/z7p30ket6k21 via Magisk app or Kitsune Mask app or KernelSU app or Apatch app or Recovery if Magisk or Kitsune Mask installed
- Install AML Magisk Module https://t.me/ryukinotes/34 only if using any other else audio mod module
- Reboot
- If you are using KernelSU, you need to allow superuser list manually all package name listed in package.txt (and your home launcher app also) (enable show system apps) and reboot afterwards
- If you are using SUList, you need to allow list manually your home launcher app (enable show system apps) and reboot afterwards

## Optionals
- https://t.me/ryukinotes/63
- Global: https://t.me/ryukinotes/35
- Stream: https://t.me/ryukinotes/52

## Troubleshootings
Global: https://t.me/ryukinotes/34

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Credits and Contributors
- @ahrion @zackptg5 Lennon
- @HuskyDG
- https://t.me/viperatmos
- https://t.me/androidryukimodsdiscussions
- You can contribute ideas about this Magisk Module here: https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


