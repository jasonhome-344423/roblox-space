# Roblox Space

[下载安装程序](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/RobloxSpace-Setup.exe) · [双语安装说明](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/Installation-Guide.html) · [English release notes](https://github.com/jasonhome-344423/roblox-space/blob/main/Release-Notes.md)

本次补齐华语与英文：主程序和监测窗口、通知设置与手机消息、错误提示和弹窗按钮、首次配置、独立 EXE 安装与卸载、目录选择、完整离线说明和源码备份恢复入口。修正英文按钮裁字，并为备份增加英文文件名入口。

主窗口选择语言后立即切换并记住设置。第三方程序、游戏、系统权限窗口和云端自动消息由各自语言设置决定；个人输入和原始系统诊断保留原文。

普通 X 关闭游戏、点击、监测、Moonlight 和主程序，保留 Duo 工作区；托盘“全部退出（包括 Duo）”关闭全部组件。运行中切到电池完全退出，接回电源不自动重开。最小化继续运行。程序退出后不再监测供电或断网。

安装：关闭空间，运行 RobloxSpace-Setup.exe，保留原安装目录和已有配对、通知设置。新 Windows 按双语安装说明 B1–B7 完成配置。便携 Moonlight 已包含，Duo 与 Roblox 需按说明另行安装。使用 Windows 11 x64 24H2 或以上，工作区为 1280 × 720、30 Hz。

没有软件更新功能，也不显示产品版本编号。需要安装时手动下载运行 EXE。SHA256SUMS.txt 包含公开文件哈希，完整源码备份留在本机，个人密钥和设置不公开。

由 ChatGPT 完全制作：本程序界面、代码和原创图标。Roblox、Duo、Moonlight 为独立第三方组件。

## 分发与排查说明

当前安装器**没有数字签名**。从本仓库发布页下载，并与同一发布的 SHA256SUMS.txt 核对；SmartScreen 步骤在双语说明开头。哈希核对不代替发布者签名，请勿关闭 Windows 保护。

Moonlight、Qt 等运行库的许可原文、版权、哈希、源码及构建资料随附于 runtime/Moonlight/licenses 和 NOTICE.txt。licenses/sources/ 实际包含 Moonlight、Qt 6.12.0 的 qtbase/qtdeclarative/qtsvg、FFmpeg 和 libplacebo 源码包，以及固定依赖构建方法和补丁。SOURCE-BUILD-NOTES.txt 说明构建输入；materials.json 记录原网址与 SHA256。安装器、本机离线源码备份及公开的 Third-Party-Notices.zip 均包含这些资料，无需仅依赖上游链接长期有效。

Healthchecks 使用仅包含本软件一个检查的**专用项目**及该项目自己的读写 Key。它的权限覆盖整个项目。说明中写明了转移旧检查、保留 Ping URL、配置新项目 Telegram 与 Key 的步骤；安装器不自动迁移现有云端设置。

托盘“关于”和每次启动首条日志记录构建短哈希和 UTC 构建时间，主界面不显示产品版本号。备份清单改为 manifest.json，ZIP 与清单路径使用正斜杠。备份根目录只保留一份完整双语说明，另保留可编辑语言源模板，华语 HTML 文件名是轻量入口。