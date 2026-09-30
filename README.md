# IranFilternetBypass

A community-maintained collection of tools, configurations, resources, and techniques for accessing the open internet from Iran despite internet filtering and censorship.

---

### ♥ Please read this:

A message from the owner: 

We love the people in iran (except the ones who love Islamic Republic), and we want to give them the freedom of the internet. **BUT** please don't sell our free configs. We get in trouble often with this and we are asking you to not sell our configs. Its okay to share them but please don't sell them. Thank you.

## 📌 What is this?

**IranFilternetBypass** collects resources that may help users in Iran access websites and services that are blocked, filtered, or disrupted.

The repository may include:

* 🔗 V2Ray / Xray configurations
* 🛡️ VPN and proxy resources
* 🌐 DNS and DoH/DoT resources
* 🌎 Connectivity around the world
* ⚡ Cloudflare and CDN-based techniques
* 📱 Android tools
* 💻 Windows tools
* 🧪 Network testing utilities
* 📚 Guides and troubleshooting information
* 📡 Information about current filtering and connectivity issues

## 📂 Repository Structure

```text
IranFilternetBypass/
│
├── configs/
│   ├── countries/
│   │   ├── vless/
│   │   ├── vmess/
│   │   ├── shadowsocks/
│   │   ├── subscriptions/
│   │   └── trojan/
│   └── ...
│
├── tools/
│   ├── windows/
│   └── android/
│
├── guides/
│   ├── android.md
│   ├── windows.md
│   └── troubleshooting.md
│
├── scripts/
│   └── ...
│
└── README.md
```

## 🔌 Supported Protocols

Depending on availability, this repository may contain resources using:

| Protocol             | Supported             |
| -------------------- | --------------------- |
| VLESS                | ✅                     |
| VMess                | ✅                     |
| Trojan               | ✅                     |
| Shadowsocks          | ✅                     |
| SOCKS5               | ✅                     |
| HTTP Proxy           | ✅                     |
| WireGuard            | ⚠️ Depends on network |
| Hysteria / Hysteria2 | ⚠️ Depends on network |
| Reality              | ⚠️ Depends on network |

Availability can vary significantly between Iranian ISPs and over time.

## 🚀 Getting Started

Choose the platform you are using.

### Windows

Recommended clients may include:

* v2rayN
* NekoBox
* sing-box-based clients

Import a supported configuration or subscription into your client and test the connection.

### Android

Possible clients include:

* V2RayNG
* NekoBox
* sing-box-based clients

Configuration files or subscription links can generally be imported directly into compatible clients.

## 🧪 Testing a Configuration

A configuration being listed in this repository does **not** guarantee that it will work for everyone.

Test:

1. DNS resolution
2. TCP connectivity
3. TLS handshake
4. Proxy connection
5. Actual HTTPS access

Example:

```powershell
nslookup example.com
```

For a basic HTTPS test:

```powershell
curl.exe -I https://example.com
```

For proxy testing:

```powershell
curl.exe -x http://127.0.0.1:10809 https://example.com
```

Change the proxy address and port to match your client.

## ⚠️ Why a Configuration May Stop Working

Iran's filtering infrastructure can change frequently.

A previously working configuration may stop working because of:

* IP blocking
* Domain blocking
* SNI filtering
* DNS poisoning
* TLS fingerprint filtering
* Port blocking
* CDN/IP changes
* Server shutdown
* Expired certificates
* ISP-specific filtering
* Temporary nationwide filtering changes

Therefore, **do not assume that a configuration is permanently functional**.

## 📡 ISP Differences

A connection that works on one Iranian ISP may fail on another.

For example, behavior can differ between:

* همراه اول (Hamrah Aval)
* ایرانسل (Irancell)
* رایتل (Rightel)
* Fixed-line ISPs
* Home broadband providers

When reporting a configuration, include the ISP if possible.

## 📝 Reporting a Working / Broken Config

If you find a configuration that works, please provide:

```text
Protocol:
ISP:
Country:
Test date:
Client:
Client version:
Network type:
Result:
Notes:
```

Example:

```text
Protocol: VLESS Reality
ISP: Hamrah Aval
Country: Iran
Test date: 2026-10-01
Client: v2rayN
Client version: 7.x
Network type: 4G
Result: Working
Notes: YouTube and Google reachable
```

Avoid publishing private credentials, server-management credentials, or other sensitive information.

## 🔐 Security

Never share:

* Private keys
* Server passwords
* SSH credentials
* API tokens
* Personal access tokens
* Private subscription URLs
* Authentication credentials

Public configurations should contain only information intended to be distributed publicly.

## 🧰 Useful Tools

Some useful tools for diagnosing connectivity include:

```text
nslookup
ping
tracert
curl
Test-NetConnection
```

Windows example:

```powershell
Test-NetConnection example.com -Port 443
```

DNS test:

```powershell
nslookup example.com
```

Route test:

```cmd
tracert example.com
```

## 📜 License

Choose a license appropriate for the contents of this repository.

For example, if most of the repository consists of original documentation and scripts, you may use the **MIT License**.

Third-party configurations, software, and documentation remain subject to their respective licenses.

---

## 📡 Donate Configurations

Have a working proxy, VPN, or V2Ray/Xray configuration that can help users in Iran? **Donate it to the project.**

You can contribute:

* 🔗 VLESS configurations
* 🔗 VMess configurations
* 🛡️ Trojan configurations
* ⚡ Shadowsocks configurations
* 🌐 Hysteria / Hysteria2 configurations
* 🔐 Reality configurations
* 📡 Working proxy servers
* 🧪 Tested ISP-specific configurations

### How to Contribute

Open a **Pull Request** and add your configuration to the appropriate directory.

Please include:

```text
Protocol:
ISP:
Country:
Config / Subscription URL:
Tested on:
Date tested:
Notes:
```

### ⚠️ Please Don't Submit

* Private or stolen credentials
* Personal accounts
* Compromised servers
* Configurations containing sensitive information
* Expired or intentionally broken configurations
* Unknown or unsafe URLs

**Every working configuration helps expand the collection. 🇮🇷**

---

### ⭐ Support the Project

If this repository helped you:

* ⭐ Star the repository
* 🐛 Report broken configurations
* 🔧 Submit improvements
* 📖 Improve the documentation

**Keep the information accurate, keep credentials private, and keep testing.**
