# PattConfig

A client-side generator to build **PattNG-compatible custom configurations** from raw VLESS and Trojan links for various Xray clients (v2rayN, Throne, and v2rayNG).

👉 **[Launch Web App](https://cherk-nevis.github.io/PattConfig/)**

---

## What is PattConfig?

The [PattNG](https://github.com/patterniha/PattNG) project introduced highly effective anti-censorship profiles based on TCP packet fragmentation and specialized TLS cipher suites.

**PattConfig** is a web-based companion tool that allows you to take standard VLESS or Trojan links, combine them with your own Clean IPs, and automatically generate fully configured JSON files matching the PattNG architecture.

---

## Features & Options

- **Configs, Links & Subscriptions**: Accepts `vless://`, `trojan://`, base64 subscriptions, raw subscription URLs (with CORS bypass), and full Xray config JSONs.
- **Smart Remarks**: Generates clean, accessible remarks (`VLESS 1, 104.21.33.59:443`).
- **Routing Rules**: Optional toggles for bypassing domestic Iran traffic, blocking QUIC (UDP 443), blocking ads, and specifying custom direct domains.
- **LAN Sharing**: Toggle `Allow LAN` to listen on `0.0.0.0` for sharing proxy access across the local network.
- **Clean Endpoints**: Set custom Clean IPs/domains, load tested sample endpoints, or fetch live auto-scanned Cloudflare clean IPs with a single click.
- **Port Selection**: Generate configurations across multiple Cloudflare HTTPS ports (`443`, `8443`, `2053`, `2083`, `2087`, `2096`).
- **DNS Configuration**: Configure remote DoH (`https://8.8.8.8/dns-query`) and domestic direct DNS servers.
- **Fragmentation (`finalmask`) & Ciphers**: Pre-loaded with PattNG's two-stage fragmentation (`tlshello` + `1-1`) and optimized cipher suites.
- **Inbound Ports**: Customize local mixed SOCKS/HTTP proxy ports (`10808`, `2080`, or custom).

---

## Client Usage

- **Copy**: Copies the configuration directly to clipboard for one-click import in your client.
- **Download**: Downloads `configs.json` for file-based import or sharing.

---

## Privacy

Runs entirely inside your browser (JavaScript only). Works offline with zero server logging or external data transfer.

---

## Acknowledgments

- [PattNG](https://github.com/patterniha/PattNG): Configuration architecture, TLS cipher selection, and fragmentation profiles.
- [NiREvil](https://github.com/NiREvil/vless): Automated live Cloudflare clean IP feeds.
