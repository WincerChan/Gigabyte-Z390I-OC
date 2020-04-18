该目录是 macOS 的内核扩展目录，应包含：

1. Lilu.kext（必须）
2. WhateverGreen.kext（必须）
3. VirtualSMC.kext（必须）
4. IntelMausi.kext（必须）：网卡驱动
5. AppleALC.kext（必须）：音频驱动
6. USBPorts.kext（必须，定制）：USB 定制驱动，如果不想[定制](https://blog.daliansky.net/Intel-FB-Patcher-tutorial-and-insertion-pose.html)，请使用 USBInjectAll.kext，否则进系统之后无法使用鼠标键盘等 USB 设备。
7. SMCProcessor.kext（非必须）：CPU 传感器驱动
8. SMCSuperIO.kext（非必须）：IO 传感器驱动
9. AirportBrcmFixup.kext（非必须）： Broadcom 的无线网卡驱动

> 如果不想定制 USB，也不想使用 USBInjectAll，可以在 ACPI 里添加 SSDT-USBX.aml 补丁，但不推荐这样做，因为 ACPI 补丁对 Windows 或是其他系统同样会生效。