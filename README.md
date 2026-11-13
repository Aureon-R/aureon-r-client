# Aureon R

Independent proxy client with Xray and sing-box. Official signed releases only. / 独立代理客户端，集成 Xray 与 sing-box。本仓库仅用于官方签名安装包和使用说明发布，不含应用开发源码。

[Download / 下载](https://github.com/Aureon-R/aureon-r-client/releases) · [Official website / 官网](https://aureonvpn.com/en/aureon-r) · [中文官网](https://aureonvpn.com/aureon-r?lang=zh)

## Self-hosted sharing / 自托管节点分享
Self-hosted sharing access is not yet publicly available. Registered users may email Aureon-vpn@proton.me with their Aureon R account username to request manual activation. Existing authorized users can continue sharing. Never include passwords, SSH credentials or recovery codes.

自托管分享权益暂未公开开放。已注册用户可发送邮件至 Aureon-vpn@proton.me，附上 Aureon R 账户名称申请人工开通。已有分享权益的用户可继续使用。请勿发送密码、SSH 凭据或恢复码。

## User guide / 使用说明

Aureon R is an independent proxy client. It does not provide official proxy nodes. Import and connection are free; self-hosted deployment is free, but users pay their own VPS provider.

Aureon R 是独立代理客户端，不提供官方代理节点。节点导入、连接及自托管部署免费，VPS 费用由用户自行承担。

### 1. Import nodes / 导入节点
In Settings, import a configuration link, text, QR code, image or subscription. Select a node in Nodes and connect. No account is required for ordinary node import and connection.

在设置中导入链接、文本、二维码、图片或订阅；在节点列表选择目标节点并连接。普通节点导入和连接无需注册登录。

### 2. Connection and DNS / 连接与 DNS
Xray and sing-box support VLESS Reality Vision, Hysteria 1/2, TUIC v5, WireGuard, AnyTLS, Trojan TLS and VMess TLS. Strict mode combines global proxy routing with encrypted DNS (DoH). View traffic, current node and DNS information in the app.

Xray 与 sing-box 双内核支持 VLESS Reality Vision、Hysteria 1/2、TUIC v5、WireGuard、AnyTLS、Trojan TLS 和 VMess TLS。严格模式结合全局代理及 DoH 加密 DNS。可在 APP 查看流量、当前节点和 DNS 信息。

### 3. Deploy your own VPS / 自托管部署
Prepare your own Debian VPS with SSH access. Register and sign in to Aureon R, open Self-hosted, enter the VPS IP, SSH username and password, select protocol and DNS, then deploy. The app installs Docker, configures the proxy and firewall, and creates the node. Additional supported protocols can be added to the same VPS. Redeploying can overwrite managed settings; removing a server deletes its managed deployment. Back up important data first.

准备自己的 Debian VPS 及 SSH 登录资料，在 APP 注册登录后进入自托管，填写 IP、SSH 用户名及密码，选择协议与 DNS，然后一键部署。APP 自动安装 Docker、配置代理服务和防火墙并生成节点。同一 VPS 可继续添加其他支持的协议。覆盖部署可能清除原有配置，删除服务器会删除 APP 管理的部署，请先备份重要资料。

### 4. Share nodes / 节点分享
With sharing access enabled, choose your self-hosted server and generate a QR code or share code. The recipient can import the share in Aureon R without an account. Each guest receives independent device credentials; a successfully claimed code cannot be reused. Owners can manage and revoke guests. Actual capacity depends on the VPS and protocol resources.

开通分享权益后，选择自托管服务器，生成二维码或分享码。接收者无需注册，可在 Aureon R 导入分享。每位访客使用独立设备凭据，成功领取后分享码失效。所有者可管理及撤销访客权限。实际规模取决于 VPS 性能和协议资源。

### 5. Encrypted backup and restore / 加密备份与恢复
Back up eligible nodes, VPS management records and local guest names to your own VPS. Keep the recovery code separately. On another phone, sign in to the same account, connect to the backup VPS and restore with the recovery code and server-held key. Existing entries are retained; missing entries are restored. Guest device keys cannot be transferred through owner backups.

将可备份节点、VPS 管理资料及本地访客名称加密备份到自己的 VPS，妥善保管恢复码。在另一部手机登录同一账号，连接备份 VPS，使用恢复码及服务端密钥进行增量恢复；已有数据不覆盖。接收端设备密钥不随分享者备份转移。

### 6. Accounts and support / 账户与客服
Register in the app. Each account supports one signed-in phone at a time. Release the old device using the website if needed. Private support messages are synchronized between the website and app.

在 APP 内注册账户，同一账号同时仅允许一台手机登录。需要换机时可在网站解除旧设备占用。网页和 APP 的私信客服会话同步。

- Full guide / 完整说明: https://aureonvpn.com/en/aureon-r/app-guide
- 中文指南: https://aureonvpn.com/aureon-r/app-guide?lang=zh
- Account center / 账户中心: https://aureonvpn.com/aureon-r/account
- Support / 联系我们: https://aureonvpn.com/en/aureon-r/contact


## Release integrity / 安装包校验
Verify SHA-256 using SHA256SUMS in each release. / 请使用每个版本附带的 SHA256SUMS 校验安装包。
