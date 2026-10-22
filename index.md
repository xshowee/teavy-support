---
title: Teavy 支持 · Support
---

# Teavy 支持

Teavy 是 iPhone、iPad 和 Android 手机、平板上的 VNC 远程桌面客户端，可以连接 macOS 屏幕共享和 TigerVNC 等标准 VNC 服务端。

问题反馈和建议请发邮件至 [dev@xshowee.com](mailto:dev@xshowee.com)，最好写明设备型号、系统版本和要连接的电脑。

[隐私政策](privacy.html)

## 下载 Android 版

Android 版暂不在 Google Play 上架，请从 [GitHub Releases](https://github.com/xshowee/teavy-support/releases/latest) 下载最新的 `teavy-版本号.apk`。

- **系统要求**：Android 10 及以上的 64 位设备。
- **安装**：用手机浏览器下载后点按安装。第一次安装时系统会要求允许浏览器“安装未知应用”。
- **更新**：有新版本时 Teavy 会提示，下载新版本后直接覆盖安装，已保存的连接和密码都会保留。**不要先卸载旧版本**：卸载会删除保存在本机的连接、密码和 SSH 密钥，无法恢复。
- **只从本页下载**：别人可以修改 Teavy 后重新打包，冒充正版。正版的签名证书 SHA-256 指纹是：

  `66:79:A5:6A:35:35:29:41:9F:C3:99:B7:0C:BD:A3:35:23:6C:F5:B8:1A:A7:53:06:00:F6:30:D2:08:92:F9:0D`

  在电脑上可以用 `apksigner verify --print-certs teavy-版本号.apk` 核对（输出的 `certificate SHA-256 digest` 与上面相同，不区分大小写和冒号）。每个版本还附有 `.sha256` 文件，可用 `shasum -a 256` 核对下载的文件是否完整。

## 常见问题

**怎样让 Mac 可以被连接？**
在 Mac 上打开“系统设置 › 通用 › 共享”，开启“屏幕共享”。在 Teavy 中添加这台 Mac 时填写它的账户名称和密码。

**怎样连接 Windows 或 Linux 电脑？**
在电脑上安装并运行 VNC 服务端（例如 TigerVNC），并为它设置 VNC 密码。在 Teavy 中添加连接时填写电脑的地址、端口（默认 5900）和 VNC 密码。

**连上 Mac 后停在锁屏界面怎么办？**
iPhone 和 iPad：点会话右上角的“更多”，选“解锁 Mac”，Teavy 会用这次登录的账户密码解锁。为了确保密码只输入到锁屏的密码框里，Teavy 会先锁屏再解锁，所以 Mac 原本没锁时会先锁上再解开。
Android：点会话工具栏上的钥匙按钮，选“输入用户密码”，Teavy 会把这次登录的账户密码输入锁屏的密码框。Mac 没有锁屏时，密码会输入到当前光标所在的地方，所以请在看到锁屏界面时再用。

**怎样从外网安全地连接？**
VNC 本身不加密。在连接设置中开启“通过 SSH 隧道连接”，画面和输入会经 SSH 加密。电脑需要开启 SSH（Mac 上是“系统设置 › 通用 › 共享 › 远程登录”）。在 Teavy 的“设置”中生成 SSH 密钥，把公钥加入电脑上的 `~/.ssh/authorized_keys`，就不必每次输入 SSH 密码。

**连接失败怎么办？**
确认手机或平板与电脑在同一网络（或通过 SSH 隧道连接），电脑上的屏幕共享或 VNC 服务已经开启，防火墙允许对应的端口。还要允许 Teavy 访问本地网络：iOS 上在“设置 › 隐私与安全性 › 本地网络”中开启；Android 上在 Teavy 的应用设置里，到“权限”中开启“附近的设备”。

---

# Teavy Support

Teavy is a VNC remote desktop client for iPhone, iPad, and Android phones and tablets. It connects to macOS Screen Sharing and standard VNC servers such as TigerVNC.

For questions and feedback, email [dev@xshowee.com](mailto:dev@xshowee.com). Please include your device model, system version, and the computer you're connecting to.

[Privacy Policy](privacy.html)

## Download for Android

Teavy for Android isn't on Google Play yet. Download the latest `teavy-<version>.apk` from [GitHub Releases](https://github.com/xshowee/teavy-support/releases/latest).

- **Requirements**: A 64-bit device running Android 10 or later.
- **Install**: Download the file in your phone's browser and tap it to install. The first time, Android asks you to allow the browser to install unknown apps.
- **Update**: Teavy lets you know when a new version is available. Download it and install it over the current version; your saved connections and passwords are kept. **Don't uninstall the old version first**: uninstalling deletes the connections, passwords, and SSH key stored on your device, and they can't be recovered.
- **Download only from this page**: Others can modify Teavy and repackage it as a fake. The genuine app's signing certificate SHA-256 fingerprint is:

  `66:79:A5:6A:35:35:29:41:9F:C3:99:B7:0C:BD:A3:35:23:6C:F5:B8:1A:A7:53:06:00:F6:30:D2:08:92:F9:0D`

  On a computer, check it with `apksigner verify --print-certs teavy-<version>.apk`: the `certificate SHA-256 digest` it prints matches the value above, ignoring case and colons. Each release also includes a `.sha256` file, so you can check the download with `shasum -a 256`.

## FAQ

**How do I make my Mac available?**
On your Mac, open System Settings › General › Sharing and turn on Screen Sharing. When adding the Mac in Teavy, enter the name and password of an account on that Mac.

**How do I connect to a Windows or Linux computer?**
Install and run a VNC server (such as TigerVNC) on the computer and set a VNC password. In Teavy, add a connection with the computer's address, port (5900 by default), and VNC password.

**My Mac is at the lock screen after connecting. What do I do?**
On iPhone and iPad: Tap More in the top-right corner of the session and choose Unlock Mac. Teavy unlocks it with the account password you logged in with. To make sure the password goes only into the lock screen's password field, Teavy locks the screen first, so if your Mac wasn't locked, it locks and then unlocks.
On Android: Tap the key button in the session toolbar and choose Type User Password. Teavy types the account password you logged in with into the lock screen's password field. If your Mac isn't locked, the password is typed wherever the cursor is, so use it only when you see the lock screen.

**How do I connect securely over the internet?**
VNC isn't encrypted. Turn on Connect Through SSH Tunnel in the connection settings to encrypt the screen and input with SSH. The computer needs SSH turned on (on a Mac: System Settings › General › Sharing › Remote Login). Generate an SSH key in Teavy's Settings and add the public key to `~/.ssh/authorized_keys` on the computer, so you don't need an SSH password each time.

**The connection fails. What should I check?**
Make sure your phone or tablet is on the same network as the computer (or connect through an SSH tunnel), Screen Sharing or the VNC server is turned on, and the firewall allows the port. Teavy also needs access to your local network: on iOS, turn it on in Settings › Privacy & Security › Local Network; on Android, open Teavy's app settings, go to Permissions, and turn on Nearby devices.
