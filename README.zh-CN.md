<p align="center"><img src="https://aureonvpn.com/images/aureon-r-launcher.webp" width="96" height="96" alt="Aureon R"></p>
<h1 align="center">Aureon R</h1>

<p align="center">你的节点，你的服务器，由你掌控。</p>

<p align="center"><a href="README.md">English</a> · <strong>简体中文</strong></p>

<p align="center"><strong><a href="https://github.com/Aureon-R/aureon-r-client/releases/latest">下载最新版 Android APK</a></strong> · <a href="https://aureonvpn.com/aureon-r?lang=zh">中文官网</a> · <a href="https://github.com/Aureon-R/aureon-r-client/discussions">用户社区</a></p>

Aureon R 是免费的 Android 独立代理客户端，支持用户自行导入节点及在自己的 Debian VPS 一键部署。集成 Xray 与 sing-box 双内核，不提供官方代理节点。

本仓库仅发布官方已签名安装包及公开使用说明，不公开应用开发源码。

## APP 界面展示

以下为实际 Android APP 截图，账户名称、私人服务器资料及访客名称已遮挡。点击图片可查看原尺寸。

<table>
<tr>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/home-zh.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/home-zh.png" width="190" alt="连接首页"></a><br><strong>连接首页</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/nodes-zh.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/nodes-zh.png" width="190" alt="节点列表"></a><br><strong>节点列表</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/selfhost-zh.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/selfhost-zh.png" width="190" alt="自托管节点"></a><br><strong>自托管节点</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/deploy-zh.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/deploy-zh.png" width="190" alt="VPS 一键部署"></a><br><strong>VPS 一键部署</strong></td>
</tr>
<tr>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/sharing-zh.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/sharing-zh.png" width="190" alt="分享与访客管理"></a><br><strong>分享与访客管理</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/backup-zh.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/backup-zh.png" width="190" alt="加密备份"></a><br><strong>加密备份</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/settings-zh.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/settings-zh.png" width="190" alt="设置与节点导入"></a><br><strong>设置与节点导入</strong></td>
</tr>
</table>

## 主要功能

- Xray 与 sing-box 双内核。
- 八种部署协议：VLESS Reality Vision、Hysteria 1、Hysteria 2、TUIC v5、WireGuard、AnyTLS、Trojan TLS、VMess TLS。
- 无需登录即可导入链接、文本、二维码、图片及订阅。
- 严格模式：全局代理与 DoH 加密 DNS。
- Debian VPS 一键 Docker 部署及自托管节点管理。
- 自托管节点分享、独立访客凭据及撤销授权。
- 在自己的 VPS 上加密备份，并进行增量恢复。
- 简体中文和英文、账户及设备管理、私信客服。

## 下载与安装

1. 在 [Releases 版本发布页面](https://github.com/Aureon-R/aureon-r-client/releases/latest) 下载已签名 Android ARM64 APK。
2. 使用附带的 SHA256SUMS 文件校验 APK 的 SHA-256。
3. 在兼容的 Android 设备上安装 APK，仅允许可信来源的安装。
4. 导入已有节点或部署自己的服务器，选择节点并连接。

## 使用说明

### 一、导入已有节点

在设置中选择链接、文本、二维码、图片或订阅导入。导入后进入节点列表选择目标节点并连接。普通节点导入和连接无需注册登录。可在设置中管理订阅并更新节点列表。

### 二、连接与 DNS

选择所需节点，点击连接。双内核支持上述八种协议。严格模式结合全局代理与 DoH 加密 DNS。首页可查看连接状态、流量及 DNS 信息，实际 DNS 出口可以通过检测功能另行核验。

### 三、自托管 VPS 一键部署

准备一台自己的 Debian VPS 及 SSH 登录资料。在 APP 注册登录后进入自托管节点，填写 VPS IP 或域名、SSH 用户名及密码，选择协议和 DNS，然后开始自动部署。APP 自动安装 Docker，配置代理服务与防火墙，并生成节点。同一 VPS 可继续添加其他支持的协议。

自托管部署免费，VPS 费用由用户自行承担。覆盖部署前请确认目标服务器并备份重要资料；覆盖部署可能清除原有受管理配置，删除服务器将删除 Aureon R 管理的部署。

### 四、节点分享与访客管理

**自托管分享权益暂未公开开放。** 已注册 Aureon R 的用户可发送邮件至 **Aureon-vpn@proton.me**，附上自己的 Aureon R 账户名称，申请人工开通。已有分享权益的用户可以继续使用。请勿发送密码、SSH 凭据或备份恢复码。

开通后，选择自托管服务器并生成二维码或分享码。接收者无需注册账户，即可在 Aureon R 导入分享节点。每位访客使用独立凭据，成功领取后分享码失效。所有者可以修改访客名称并撤销单独访客授权。实际分享规模取决于 VPS 性能与协议资源。

### 五、加密备份与恢复

将可备份节点、VPS 管理资料及本地访客名称加密备份至自己的 VPS，另行妥善保存恢复码。更换手机后登录同一账号，连接备份 VPS，使用恢复码及服务端密钥进行增量恢复。已有数据不覆盖，缺失数据进行恢复。接收端设备密钥不会随分享者备份转移，访客更换设备后需要重新获得分享授权。

### 六、账户、设备与客服

在 APP 内注册账户，同一账号同时仅允许一台手机登录。更换设备前退出旧手机，或者通过网站解除旧设备占用。官网与 APP 共用私信客服会话和回复记录。

- [完整 APP 功能说明](https://aureonvpn.com/aureon-r/app-guide?lang=zh)
- [官方下载中心](https://aureonvpn.com/aureon-r/downloads?lang=zh)
- [账户中心](https://aureonvpn.com/aureon-r/account?lang=zh)
- [联系我们](https://aureonvpn.com/aureon-r/contact?lang=zh)
- [用户讨论区](https://github.com/Aureon-R/aureon-r-client/discussions)
- [提交故障报告](https://github.com/Aureon-R/aureon-r-client/issues)

请勿在公开讨论区发布账户隐私资料、私钥、节点或订阅凭据、SSH 凭据及恢复码。
