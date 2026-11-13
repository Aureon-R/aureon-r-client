<p align="center"><img src="https://aureonvpn.com/images/aureon-r-launcher.webp" width="96" height="96" alt="Aureon R"></p>
<h1 align="center">Aureon R</h1>

<p align="center">Your nodes. Your servers. Your control.</p>

<p align="center"><strong>English</strong> · <a href="README.zh-CN.md">简体中文</a></p>

<p align="center"><strong><a href="https://github.com/Aureon-R/aureon-r-client/releases/latest">Download latest Android APK</a></strong> · <a href="https://aureonvpn.com/en/aureon-r">Official website</a> · <a href="https://github.com/Aureon-R/aureon-r-client/discussions">Community</a></p>

Aureon R is a free Android proxy client for user-provided nodes and self-hosted Debian VPS deployments. It integrates Xray and sing-box. Aureon R does not provide managed proxy nodes.

This repository distributes official signed installation packages and public documentation. The application development source code is not public.

## App screenshots

Actual Android app screenshots. Account names, private server details and guest names have been redacted. Select an image to view it at full size.

<table>
<tr>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/home-en.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/home-en.png" width="190" alt="Connection"></a><br><strong>Connection</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/nodes-en.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/nodes-en.png" width="190" alt="Node management"></a><br><strong>Node management</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/selfhost-en.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/selfhost-en.png" width="190" alt="Self-hosted nodes"></a><br><strong>Self-hosted nodes</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/deploy-en.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/deploy-en.png" width="190" alt="One-click VPS deployment"></a><br><strong>One-click VPS deployment</strong></td>
</tr>
<tr>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/sharing-en.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/sharing-en.png" width="190" alt="Sharing and guests"></a><br><strong>Sharing and guests</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/backup-en.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/backup-en.png" width="190" alt="Encrypted backup"></a><br><strong>Encrypted backup</strong></td>
<td align="center"><a href="https://aureonvpn.com/images/aureon-r-screenshots/settings-en.png"><img src="https://aureonvpn.com/images/aureon-r-screenshots/settings-en.png" width="190" alt="Settings and import"></a><br><strong>Settings and import</strong></td>
</tr>
</table>

## Main features

- Xray and sing-box dual cores.
- Eight deployment protocols: VLESS Reality Vision, Hysteria 1, Hysteria 2, TUIC v5, WireGuard, AnyTLS, Trojan TLS and VMess TLS.
- Import links, text, QR codes, images and subscriptions without signing in.
- Strict mode: global proxy routing and encrypted DNS (DoH).
- One-click Docker deployment and management on your own Debian VPS.
- Authorized self-hosted node sharing, independent guest credentials and revocation.
- Encrypted backups stored on your own VPS, with incremental restore.
- Simplified Chinese and English; account and device management; private support.

## Download and installation

1. Download the signed Android ARM64 APK from [Releases](https://github.com/Aureon-R/aureon-r-client/releases/latest).
2. Verify the SHA-256 checksum against the accompanying SHA256SUMS file.
3. Install the APK on a compatible Android device. Only allow installation from the trusted source you use.
4. Import your nodes or deploy on your own server, select a node, then connect.

## User guide

### 1. Import existing nodes

Open Settings, select a link, text, QR code, image or subscription import option. After importing, open Nodes, select the desired node and connect. Ordinary node import and connection do not require registration. Manage subscriptions in Settings to update the node list.

### 2. Connection and DNS

Select the desired node and use the connection button. The dual cores support the protocols listed above. Strict mode combines global proxy routing with encrypted DNS over HTTPS. The home screen displays connection status, traffic and DNS information; actual DNS resolver detection may require a separate test.

### 3. Deploy your own VPS

Prepare a Debian VPS and SSH access. Register and sign in to Aureon R, open Self-hosted, enter the VPS IP or hostname, SSH username and password, choose a protocol and DNS, and start deployment. The app installs Docker and configures the proxy service and firewall. Add further supported protocols to the same VPS as needed.

Self-hosted deployment is free; you pay your VPS provider directly. Confirm the target server and back up important data before redeploying or removing services. Redeployment can overwrite the existing managed deployment, and deleting a server removes the deployment managed by Aureon R.

### 4. Sharing and guest management

Self-hosted sharing access is not yet publicly available. Registered users may request manual activation by emailing **Aureon-vpn@proton.me** with their Aureon R account username. Existing authorized users can continue sharing. Do not include account passwords, SSH credentials or backup recovery codes.

Once authorized, choose a self-hosted server and generate a QR code or share code. The recipient imports the share in Aureon R without creating an account. Each guest has independent credentials. A successfully claimed share code cannot be reused. The owner can rename or revoke individual guests. Actual capacity depends on VPS and protocol resources.

### 5. Encrypted backup and restore

Back up eligible nodes, VPS management records and local guest names to your own VPS. Keep the recovery code separately. On another phone, sign in to the same account, connect to the backup VPS and restore using the recovery code and server-held key. Existing entries are retained and missing entries are restored. Guest device keys are not transferred through owner backups; recipients need new sharing authorization on another device.

### 6. Accounts and support

Register in the app. Each account permits one signed-in phone at a time. Sign out of the previous phone or release it through the website before moving to a new device. The website and app share the same private support conversation.

- [Full app guide](https://aureonvpn.com/en/aureon-r/app-guide)
- [Official download center](https://aureonvpn.com/en/aureon-r/downloads)
- [Account center](https://aureonvpn.com/aureon-r/account?lang=en)
- [Contact support](https://aureonvpn.com/en/aureon-r/contact)
- [Community discussions](https://github.com/Aureon-R/aureon-r-client/discussions)
- [Report an issue](https://github.com/Aureon-R/aureon-r-client/issues)

Please do not publish account details, private keys, node or subscription credentials, SSH credentials or recovery codes in public discussions.
