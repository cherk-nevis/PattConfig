# PattConfig

A client-side generator to build **PattNG-compatible custom configurations** from raw VLESS and Trojan links for various Xray clients (v2rayN, Throne, and v2rayNG).

👉 **[Launch Web App](https://cherk-nevis.github.io/PattConfig/)**

---

## What is PattConfig?

The [PattNG](https://github.com/patterniha/PattNG) project introduced highly effective anti-censorship profiles based on TCP packet fragmentation and specialized TLS cipher suites.

**PattConfig** is a web-based companion tool that allows you to take standard VLESS or Trojan links, combine them with your own Clean IPs, and automatically generate fully configured JSON files matching the PattNG architecture.

---

## Features & Options

- **VLESS & Trojan Links**: Paste single or multiple `vless://` and `trojan://` URLs.
- **Clean Endpoints**: Set custom Clean IPs/domains to bypass blocked default CDN addresses.
- **Port Selection**: Generate configurations across multiple Cloudflare HTTPS ports (`443`, `8443`, `2053`, `2083`, `2087`, `2096`).
- **Fragmentation (`finalmask`) & Ciphers**: Pre-loaded with PattNG's two-stage fragmentation (`tlshello` + `1-1`) and optimized cipher suites.
- **Inbound Ports**: Customize local SOCKS/HTTP proxy ports.

---

## Client Usage

- **Copy (v2rayN / Throne)**: Copies the configuration directly for one-click clipboard import.
- **Download (v2rayNG)**: Downloads `configs.json` for file-based import in v2rayNG.

---

## Privacy

Runs entirely inside your browser (JavaScript only). Works offline with zero server logging or external data transfer.

---

## Acknowledgements

Core fragmentation profiles, cipher selection, and routing rules are based on the [PattNG](https://github.com/patterniha/PattNG) project.
