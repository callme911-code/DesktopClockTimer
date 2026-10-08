# DesktopClockTimer 发布维护规则

## 仓库定位

该公开仓库仅用于：

1. 展示产品信息和版本记录；
2. 托管正式二进制附件；
3. 为应用内“检查更新”提供稳定地址。

完整源码、软著材料和 Microsoft Store 专用源码包应私下保存，不直接上传到公开仓库。

## 每个正式版本的固定附件

```text
DesktopClockTimer.exe
DesktopClockTimer_Portable.zip
SHA256SUMS.txt
```

`SHA256SUMS.txt` 只列本次 Release 实际上传的文件，每条记录必须保持在同一行：

```text
<64位SHA-256><两个空格><文件名>
```

## 正确发布顺序

1. 在 `main` 更新 README、CHANGELOG 和该版本的发布说明。
2. 提交并记录完整 commit SHA。
3. 从同一份已留存源码构建 EXE 和便携包。
4. 对最终附件计算 SHA-256。
5. 在上述 commit 上创建新标签。
6. 创建正式 Release，并上传三个固定名称附件。
7. 从 GitHub 公开地址重新下载三个附件。
8. 执行 `sha256sum -c SHA256SUMS.txt` 或等效 PowerShell 校验。
9. 确认 `/releases/latest` 指向新版本，且程序内“检查更新”可正常识别。

## 标签规则

- 已公开的旧标签不要移动或强制覆盖。
- 当前 `v7.2.0` 与 `v7.3.0` 都指向最初的 README 提交，此历史问题不建议通过强制改标签处理。
- 从下一个维护版开始（建议 `v7.3.1`），先提交版本资料，再让标签指向该版本提交。

## Microsoft Store 版

- Store 版关闭 GitHub 自替换更新，由 Microsoft Store 负责更新。
- Store 包版本、Identity 和 Publisher 必须与 Partner Center 一致。
- Store MSIX、GitHub EXE 和各自校验文件不得混用。

