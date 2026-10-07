---
title: Teavy 支持 · Support
---

# Teavy 支持

Teavy 是 iPhone 和 iPad 上的 VNC 远程桌面客户端，可以连接 macOS 屏幕共享和 TigerVNC 等标准 VNC 服务端。

问题反馈和建议请发邮件至 [dev@xshowee.com](mailto:dev@xshowee.com)，最好写明设备型号、系统版本和要连接的电脑。

[隐私政策](privacy.html)

## 常见问题

**怎样让 Mac 可以被连接？**
在 Mac 上打开“系统设置 › 通用 › 共享”，开启“屏幕共享”。在 Teavy 中添加这台 Mac 时填写它的账户名称和密码。

**怎样连接 Windows 或 Linux 电脑？**
在电脑上安装并运行 VNC 服务端（例如 TigerVNC），并为它设置 VNC 密码。在 Teavy 中添加连接时填写电脑的地址、端口（默认 5900）和 VNC 密码。

**连上 Mac 后停在锁屏界面怎么办？**
点会话右上角的“更多”，选“解锁 Mac”，Teavy 会用这次登录的账户密码解锁。为了确保密码只输入到锁屏的密码框里，Teavy 会先锁屏再解锁，所以 Mac 原本没锁时会先锁上再解开。

**怎样从外网安全地连接？**
VNC 本身不加密。在连接设置中开启“通过 SSH 隧道连接”，画面和输入会经 SSH 加密。电脑需要开启 SSH（Mac 上是“系统设置 › 通用 › 共享 › 远程登录”）。在 Teavy 的“设置”中生成 SSH 密钥，把公钥加入电脑上的 `~/.ssh/authorized_keys`，就不必每次输入 SSH 密码。

**连接失败怎么办？**
确认 iPhone 或 iPad 与电脑在同一网络（或通过 SSH 隧道连接），电脑上的屏幕共享或 VNC 服务已经开启，防火墙允许对应的端口；并在 iOS 的“设置 › 隐私与安全性 › 本地网络”中允许 Teavy 访问本地网络。

---

# Teavy Support

Teavy is a VNC remote desktop client for iPhone and iPad. It connects to macOS Screen Sharing and standard VNC servers such as TigerVNC.

For questions and feedback, email [dev@xshowee.com](mailto:dev@xshowee.com). Please include your device model, iOS version, and the computer you're connecting to.

[Privacy Policy](privacy.html)

## FAQ

**How do I make my Mac available?**
On your Mac, open System Settings › General › Sharing and turn on Screen Sharing. When adding the Mac in Teavy, enter the name and password of an account on that Mac.

**How do I connect to a Windows or Linux computer?**
Install and run a VNC server (such as TigerVNC) on the computer and set a VNC password. In Teavy, add a connection with the computer's address, port (5900 by default), and VNC password.

**My Mac is at the lock screen after connecting. What do I do?**
Tap More in the top-right corner of the session and choose Unlock Mac. Teavy unlocks it with the account password you logged in with. To make sure the password goes only into the lock screen's password field, Teavy locks the screen first, so if your Mac wasn't locked, it locks and then unlocks.

**How do I connect securely over the internet?**
VNC isn't encrypted. Turn on Connect Through SSH Tunnel in the connection settings to encrypt the screen and input with SSH. The computer needs SSH turned on (on a Mac: System Settings › General › Sharing › Remote Login). Generate an SSH key in Teavy's Settings and add the public key to `~/.ssh/authorized_keys` on the computer, so you don't need an SSH password each time.

**The connection fails. What should I check?**
Make sure your iPhone or iPad is on the same network as the computer (or connect through an SSH tunnel), Screen Sharing or the VNC server is turned on, and the firewall allows the port. Also allow Teavy to access the local network in iOS Settings › Privacy & Security › Local Network.
