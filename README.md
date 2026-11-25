# APT Enter plugin downloads

A backup download channel for browser tools on the [APT Enter Store](https://aptenter.com/plugins/). This repository contains distribution packages and installation notes. It does not contain the projects' development history.

| Tool | GitHub release | Official APT page |
| --- | --- | --- |
| Asset CSV Export for Hudu | [Chrome test build v1.0.1](https://github.com/AugustPT/apt-enter-downloads/releases/tag/hudu-v1.0.1) | [Product guide and help](https://aptenter.com/hudu/export/) |
| Bulk Customs Editor for ShipStation | [Chrome build v1.0.0](https://github.com/AugustPT/apt-enter-downloads/releases/tag/shipstation-v1.0.0) | [Product guide and demo](https://aptenter.com/shipstation/bulk-customs/) |

For ShipStation, prefer the [Chrome Web Store](https://chromewebstore.google.com/detail/bulk-customs-editor-for-s/kjmnfgpmclpogjmadbfcjnmnjlbliljj) for regular installation and updates. The ShipStation ZIP is a manual-install backup; live changes still require store activation. The Hudu ZIP is a specific Chrome test build, not a claim that it is the latest Hudu version.

### Install a manual Chrome build

1. Open the release and download the ZIP listed under **Assets**. Do not use GitHub's automatically generated **Source code** archives.
2. Unzip it. Open `chrome://extensions` in desktop Chrome and turn on **Developer mode**.
3. Select **Load unpacked**, then select the extracted folder containing `manifest.json`. Keep that folder in place while using the extension.

Only install a build you trust. If a managed browser blocks this type of installation, follow your organization's policy. Manual installations do not update themselves. See the [APT install guide](https://aptenter.com/plugins/#install) and [Chrome's own instructions](https://developer.chrome.com/docs/extensions/get-started/tutorial/hello-world#load-unpacked).

### Check a download

Each release includes a `SHA256SUMS.txt` file. To verify a ZIP, compare its SHA-256 hash with the one in that file. On macOS or Linux, run `shasum -a 256 <file.zip>`. On Windows PowerShell, run `Get-FileHash <file.zip> -Algorithm SHA256`.

For help, use the product guide above. APT Enter develops these tools independently of Hudu and ShipStation.
