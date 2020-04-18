该目录是 EFI 驱动文件目录，一般包括：

1. ApfsDriverLoader.efi（必须）：APFS 文件系统支持
2. HFSPlus.efi（必须）
3. OpenRuntime.efi（必须）
4. OpenUsbKbDxe.efi（必须）
5. NdkBootPicker.efi（非必须，官方 GUI 主题）
6. OpenCanopy.efi（非必须，第三方 GUI 主题）

⚠️：如果配置了官方主题，需要在 OC 文件夹（当前目录的父文件夹）内创建 Icons 文件夹，包含主题的图片。

