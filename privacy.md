---
title: Teavy 隐私政策 · Privacy Policy
---

# Teavy 隐私政策

生效日期：2026 年 11 月 15 日

本政策适用于 iPhone、iPad 版和 Android 版 Teavy。Teavy 不收集、不存储、也不向开发者或任何第三方发送你的个人数据。

- **连接信息**：你保存的连接（名称、地址、端口、用户名、SSH 设置）存在你的设备上。iPhone 和 iPad 版经你自己的 iCloud 账户在你的设备间同步；Android 版不经任何云服务同步，也不参与 Android 的备份和设备迁移。开发者无法访问这些数据。
- **密码和密钥**：VNC 密码、Mac 账户密码、SSH 密码和 SSH 私钥只存在你的设备上，开发者无法访问。iPhone 和 iPad 版存在 iOS 钥匙串中，开启 iCloud 钥匙串时随之同步；Android 版加密后保存，加密密钥由 Android Keystore 保管、不会离开设备，卸载 Teavy 后无法恢复。
- **远程画面和输入**：Teavy 直接连接你指定的电脑，画面、键盘输入和剪贴板只在你的设备和那台电脑之间传输，不经过开发者的服务器。
- **本地网络**：Teavy 请求本地网络权限，只用于发现和连接局域网中的电脑。
- **剪贴板**：iPhone 和 iPad 版只有在你点“发送剪贴板”时才读取剪贴板，并把其中的文字和图片发送给你正在连接的电脑。Android 版在连接期间、Teavy 处于前台时，会把本机剪贴板中的文字发送给正在连接的电脑；连接的是 Mac 时，剪贴板中不超过 10 MB 的图片也会发送。远程电脑复制的文字会写入本机剪贴板，连接的是 Mac 时还包括图片。
- **语音输入**：你在文本输入面板点麦克风时，Teavy 请求使用麦克风（iPhone 和 iPad 版还请求语音识别权限），录音只用来把你说的话转成文字，文字留在输入框里，由你决定是否发送。设备支持本机识别时在设备上识别，录音不离开设备；否则交给系统的语音识别服务（iPhone 和 iPad 上是 Apple，Android 上是系统设置的识别服务，例如 Google），录音可能经网络发给该服务，适用它的隐私政策。Teavy 不保存录音，也不发给开发者。
- **检查更新（Android 版）**：从本站下载的 Android 版每天打开时最多一次向 GitHub 查询最新的版本号，你也可以手动检查；可在 Teavy 的“设置 › 关于”中关闭自动检查。请求不包含关于你或你的设备的任何信息，但 GitHub 会像处理任何网络请求一样看到你的 IP 地址，这适用 [GitHub 的隐私声明](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement)。
- Teavy 不含广告、分析或跟踪代码。

本政策如有变更，会更新在本页并修改生效日期。如有疑问，请联系 [dev@xshowee.com](mailto:dev@xshowee.com)。

---

# Teavy Privacy Policy

Effective date: November 15, 2026

This policy covers Teavy for iPhone and iPad and Teavy for Android. Teavy doesn't collect, store, or send your personal data to the developer or any third party.

- **Connections**: The connections you save (name, address, port, username, SSH settings) are stored on your device. On iPhone and iPad, they sync across your devices through your own iCloud account. On Android, they aren't synced through any cloud service and aren't included in Android backups or device transfers. The developer can't access them.
- **Passwords and keys**: VNC passwords, Mac account passwords, SSH passwords, and your SSH private key stay on your device, and the developer can't access them. On iPhone and iPad, they're stored in the iOS keychain and sync with iCloud Keychain if it's turned on. On Android, they're encrypted with a key kept in the Android Keystore, which never leaves your device, and they can't be recovered after you uninstall Teavy.
- **Remote screen and input**: Teavy connects directly to the computers you specify. The screen, keyboard input, and clipboard travel only between your device and that computer, never through the developer's servers.
- **Local network**: Teavy asks for local network access only to find and connect to computers on your network.
- **Clipboard**: On iPhone and iPad, Teavy reads your clipboard only when you tap Send Clipboard, and sends its text and images to the computer you're connected to. On Android, while you're connected and Teavy is in the foreground, text on your device's clipboard is sent to the computer you're connected to; when that computer is a Mac, images up to 10 MB are sent too. Text copied on the remote computer is placed on your device's clipboard, along with images when it's a Mac.
- **Voice input**: When you tap the microphone in the text input panel, Teavy asks to use the microphone (and, on iPhone and iPad, for speech recognition permission). Audio is used only to turn what you say into text, which stays in the input field until you choose to send it. If your device supports on-device recognition, speech is recognized on the device and the audio never leaves it. Otherwise it's handled by the system's speech recognition service (Apple on iPhone and iPad; on Android, the service set in system settings, such as Google), and audio may be sent over the network to that service under its privacy policy. Teavy doesn't keep recordings or send them to the developer.
- **Update checks (Android)**: Teavy for Android downloaded from this site asks GitHub for the latest version number at most once a day when it opens, and you can also check manually. You can turn off automatic checks in Teavy's Settings › About. The request contains no information about you or your device, but GitHub sees your IP address as it does for any web request, which is covered by [GitHub's privacy statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).
- Teavy contains no advertising, analytics, or tracking code.

If this policy changes, the update will be posted on this page with a new effective date. Questions? Contact [dev@xshowee.com](mailto:dev@xshowee.com).

[返回 Teavy 支持 · Back to Teavy Support](./)
