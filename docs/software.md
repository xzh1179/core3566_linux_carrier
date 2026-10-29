# Software and display integration

The prototype uses Armbian (Debian 13 / Trixie family). A Linux display stack for this carrier includes:

1. A bootable image specifically compatible with Luckfox Core3566.
2. A base device tree matching that image/kernel.
3. A board- and display-specific device-tree overlay (or a matching complete DTB).
4. LCD reset/init/timing and MIPI DSI lane configuration.
5. Backlight PWM configuration and boot-time service.

**No universal "NV3051D DTBO" is promised.** Binary overlays are tied to the matching kernel/base device tree and integration method. The exact image identifier, overlay filename and install commands will be supplied with the verified developer package.

Please do not replace the system's active DTB with files from unrelated images. Keep a backup and a recovery path before testing custom overlays.

## Public demonstration

This repository will host photos, a short video and a reproducibility summary after the clean-install test. It intentionally does not contain the paid overlay or integration script.
