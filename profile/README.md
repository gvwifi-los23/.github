# LineageOS 23.2 for the Samsung Galaxy View (SM-T670)

Unofficial **LineageOS 23.2 (Android 16)** for the Wi-Fi **Galaxy View SM-T670** (`gvwifi`):
an 18.4" Exynos 7580 tablet from 2015, running a Linux 3.10 kernel with the backports Android 16
needs. Built on the [`github.com/gvwifi`](https://github.com/gvwifi) bring-up trees.

| Repo | What |
|---|---|
| [**lineage-gvwifi**](https://github.com/gvwifi-los23/lineage-gvwifi) | The ROM: local manifest, the patch series (kernel, device trees, frameworks, ART, …), build scripts and docs |
| [**twrp-gvwifi**](https://github.com/gvwifi-los23/twrp-gvwifi) | TWRP 3.7.1 (twrp-14.1) with automatic file-based-encryption decryption, working Data backup/restore and Format Data |
| [**lineage-recovery-gvwifi**](https://github.com/gvwifi-los23/lineage-recovery-gvwifi) | The LineageOS recovery built from the ROM tree: build, flashing and known quirks |
| [**microg-companion-gvwifi**](https://github.com/gvwifi-los23/microg-companion-gvwifi) | microG Companion built with Play Age Signals, which the ROM allowlists |

## Status
- Unofficial and maintained by one person; in daily use on the maintainer's tablet.
- Working: Wi-Fi, Bluetooth, GPS, audio, video playback (hardware composition), MTP file transfer,
  SELinux enforcing, release-key signed updates.
- **No accelerometer** on this tablet: rotation is a landscape/portrait quick-settings toggle.
- Charges only from the 19 V barrel adapter; micro-USB is data only.
- Every change and the reason for it is documented in
  [`lineage-gvwifi/docs/BUILD-KIT.md`](https://github.com/gvwifi-los23/lineage-gvwifi/blob/main/docs/BUILD-KIT.md).

## Flashing
See [`docs/FLASHING.md`](https://github.com/gvwifi-los23/lineage-gvwifi/blob/main/docs/FLASHING.md).
Coming from stock firmware erases the tablet; back up EFS first. Tested on bootloader T670UEU2APJ1 (US).

## Licenses
Patches follow the license of the project they modify (kernel: GPL-2.0; AOSP/LineageOS/TWRP/microG:
Apache-2.0). Signing keys are not published.
