# Roblox Space

[English](README.md) · 华语

把 Roblox 独立工作区、每秒点击、掉线监测和手机提醒集中在一个窗口的 Windows 软件。

**[下载安装程序](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/RobloxSpace-Setup.exe)** · **[下载完整双语安装说明](https://github.com/jasonhome-344423/roblox-space/releases/latest/download/Installation-Guide.html)** · [发布与全部附件](https://github.com/jasonhome-344423/roblox-space/releases/latest)

由 ChatGPT 完全制作：本程序的界面、代码和原创图标。Roblox、Duo 和 Moonlight 为独立第三方组件，保留各自的作者归属和许可。

## 安装和使用

1. 下载安装 EXE，在安装窗口右上角选择华语或 English。
2. 已有安装：先关闭空间，继续使用原安装目录，配对和手机通知资料会保留。
3. 新 Windows：下载 HTML 安装说明，在顶部选择华语，按 B1 到 B7 完成系统、Duo、账户权限、工作区、配对和 Roblox 登录。便携 Moonlight 已包含，无需另外安装。
4. 双击桌面 Roblox Space，Windows 权限确认选“是”。
5. 进入游戏，每次新启动后用截图确认一个安全点击位置，再按 F6 开关每秒一次点击。打字或移动前停止自动点击，再选“键盘输入”。

需要 Windows 11 x64 24H2 或以上。保持内存完整性开启，Process Patching 和 HDR 关闭。工作区使用 1280 × 720、30 Hz；不承诺免费组件能提供 60/120 Hz。

## 完整双语

主窗口、监测窗口、点击状态、选点窗口、通知设置、本程序发出的手机消息、弹窗按钮、首次配置、安装程序、目录选择和卸载程序均支持华语与英文。主窗口切换立即生效并记住选择。HTML 说明也可独立切换语言；备份命令和结果提供双语文字。

系统权限确认、游戏、Duo、Moonlight、Telegram 和 Healthchecks 自身页面或自动消息使用它们各自的语言设置。技术标识、路径、网址、密码、密钥和原始系统诊断保留原文。

## 启动、退出和供电

- 最小化：游戏、监测与点击继续运行。
- 普通 X：关闭游戏、点击、监测、Moonlight 和主程序，保留 Duo 工作区供下次快速启动。
- 全部退出：在程序开着时，右键托盘图标，选择“全部退出（包括 Duo）”。
- 运行中切到电池：全部退出。接回电源不会自动打开。
- 主程序已关闭时不再监测供电或断网。重启 Windows 或完全关闭 Duo 后，下次需要重新建立工作区。

启动耗时随系统状态变化，保留工作区一般能缩短下次启动时间。

## 手机提醒

通知设置可绑定 Telegram 机器人，发送电池切换、电脑网络和 Roblox 掉线提醒。Healthchecks 在最后一次收到电脑心跳后计算约两分钟，电脑完全断网时由云端发消息；它不等待 Roblox 掉线。手机必须能联网，并允许 Telegram 通知。

连接待确认或超时不等于 Token 过期；后台会自动重试。正常退出会尝试暂停云端检查，程序关闭期间不会监测断网。完整绑定和测试步骤见双语安装说明。

## 安装、备份和校验

本程序没有软件更新按钮、自动检查、更新提醒、安装器下载或导入功能。需要重新安装时，在浏览器下载 EXE，关闭空间后手动运行。

发布附件 SHA256SUMS.txt 提供文件校验。完整源码备份留在本机，不公开个人设置、密码、Token、API Key、配对证书、私钥或日志。源码备份包括可重建的程序、安装和卸载源码、干净的运行组件、双语说明，以及 Install.cmd / 安装.cmd、Rebuild.cmd / 重建程序.cmd、Verify-Backup.cmd / 校验备份.cmd。

内部账户 RobloxSpaceBeta、Duo 实例 RobloxBeta 是正式版兼容名称，不是另一个 Beta 程序，请保留。
