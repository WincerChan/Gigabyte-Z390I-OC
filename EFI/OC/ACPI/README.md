该目录包含 ACPI 补丁：

1. SSDT-PLUG.aml 用于提供原生的电源管理
2. SSDT-PMC.aml 用于开启 Z390 主板上原生的 NVRAM

DSDT.aml 为技嘉 Z390I 主板的文件，不用在 `config.plist` 加载，但定制 SSDT-PMC 和定制 USB 时需要用到。

》 提取方法：使用 Clover 引导：在引导界面按 F4。

如果进系统发现 USB 设备都失灵，请考虑在 Kexts 文件夹中添加 USBPorts.kext（定制）或者 USBInjectAll.kext。

**不推荐在当前目录使用 SSDT-USBX.aml。**

