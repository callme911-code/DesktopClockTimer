# Desktop Clock Timer

轻量级 Windows x64 桌面时钟、秒表和倒计时工具。

## 当前正式版

- 版本：`v7.3.0`
- 适用系统：Windows 10 / Windows 11（x64）
- 发布渠道：GitHub Releases
- 更新方式：应用内“检查更新”读取本仓库的最新正式 Release

## 下载

- [最新版 EXE](https://github.com/callme911-code/DesktopClockTimer/releases/latest/download/DesktopClockTimer.exe)
- [最新版便携包](https://github.com/callme911-code/DesktopClockTimer/releases/latest/download/DesktopClockTimer_Portable.zip)
- [最新版 SHA-256 清单](https://github.com/callme911-code/DesktopClockTimer/releases/latest/download/SHA256SUMS.txt)
- [全部版本记录](https://github.com/callme911-code/DesktopClockTimer/releases)

## 主要功能

- 桌面时钟、秒表和倒计时
- 窗口置顶、自由缩放和圆球收起状态
- 倒计时声音与震动提醒
- 十二种主题色、自定义字体与背景图
- 计算器、截图、系统静音、网址和自定义快捷方式
- 简体中文、英语、日语、韩语、西班牙语、法语和德语
- 从 `v7.3.0` 起支持应用内检查更新、SHA-256 校验、备份替换和失败回滚

## 校验下载文件

下载 `SHA256SUMS.txt` 后，可在 PowerShell 中执行：

```powershell
Get-FileHash .\DesktopClockTimer.exe -Algorithm SHA256
Get-FileHash .\DesktopClockTimer_Portable.zip -Algorithm SHA256
```

将结果与 `SHA256SUMS.txt` 中对应文件的摘要比较。两者必须完全一致。

## 发布说明

本仓库是 Desktop Clock Timer 的公开下载与自动更新仓库，正式程序放在 GitHub Releases 中。开发源码、软著材料和 Microsoft Store 专用构建材料单独留存，不在本公开仓库发布。

GitHub 便携版通过 GitHub Releases 更新；Microsoft Store 版由 Microsoft Store 管理更新，两种发行渠道互不替换。

## 联系

- 开发者：`callme911`
- 支持邮箱：`wapr@qq.com`
