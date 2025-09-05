# Unihertz Gargoyle LineageOS - Verizon Vendor Blob Integration (Untested)

## ⚠️ Warning
This is an **untested modification**. It may cause bootloops, network issues, or permanent device damage. Proceed only if you have full backups and recovery tools (SP Flash Tool with stock ROM).

## What I Did
- Pulled **all vendor blobs and telephony-related files** directly from the **Unihertz Titan Pocket stock ROM**.
- Integrated these files into the Gargoyle LineageOS device tree to address **Verizon "No Service" and VoLTE issues**.
- Structured blobs under `prebuilt/verizon_vendor_blobs/` with proper library, binary, config, and init script placement.
- Updated the build system (`device.mk`) to include these vendor components.

## Status
- **Not tested on hardware**
- Built against stock firmware `2023010520_g66v71c2k_dfl_tee` (Android 11, MT6771, Titan Pocket)
- Expected to help with Verizon authentication, VoLTE, and IMS services

## Next Steps
- Developers can try building Gargoyle with this device tree.
- Full testing is needed: SIM detection, calls, SMS, LTE data, VoLTE/VoWiFi.

## Credits
- **rumplestilzken** – Original Gargoyle LineageOS development
- **PHH-Treble team** – GSI framework
- **LineageOS team** – Base Android distribution
- **MediaTek** – Original vendor components
- **Unihertz community** – Testing and feedback

## Disclaimer
This project is **for developers only**. It is experimental, unverified, and may brick your device. Use entirely at your own risk.

