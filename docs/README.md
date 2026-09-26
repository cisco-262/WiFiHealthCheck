<p align="center">
  <img src="/docs/assets/images/app-logo.png" alt="WiFi Health Check Logo" width="120">
</p>

# WiFi Health Check

**Discover. Diagnose. Understand Your Local Network.**  
**发现、诊断并理解你的本地网络。**

WiFi Health Check is a privacy-first iPhone and iPad app for local WiFi and LAN diagnostics. It combines connection checks, LAN device discovery, port scanning, service identification, TCP stability testing, roaming analysis, and Bonjour / mDNS discovery in one focused tool.

WiFi Health Check 是一款面向 iPhone 与 iPad 的隐私优先型本地 WiFi 与局域网诊断工具，将网络连通性检查、局域网设备发现、端口扫描、服务识别、TCP 稳定性测试、WiFi 漫游分析以及 Bonjour / mDNS 服务发现整合到一个轻量工具中。

<br>

[![App Store](https://img.shields.io/badge/App_Store-Download-0D96F6?logo=apple&logoColor=white)](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)
[![Website](https://img.shields.io/badge/Website-wifi.opshome.run-2EA866)](https://wifi.opshome.run)
[![Platform](https://img.shields.io/badge/Platform-iPhone_%2B_iPad-lightgrey?logo=apple)](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)
[![Privacy](https://img.shields.io/badge/Diagnostics-Local_First-success)](https://wifi.opshome.run/privacy/)
[![Account](https://img.shields.io/badge/Account-Not_Required-blue)](https://wifi.opshome.run)

<br>

---

## v1.5 Update

WiFi Health Check v1.5 expands the app from WiFi troubleshooting into broader local-network visibility and diagnostics.

### What’s new

- **LAN Scan enhancements** for discovering devices on the local network
- **Port Scanner** for checking available TCP services on discovered hosts
- **Configurable scan concurrency** for faster or more conservative scans
- **Subnet mask selection** for more flexible LAN discovery
- **Expanded device and service fingerprints**
- Better identification for NAS software, media services, Windows / Windows Server, Linux, databases, Portainer, Kubernetes, Bonjour services, and other common infrastructure
- **Single PRO upgrade** for advanced LAN scanning controls
- Improved scan-state handling to prevent accidental navigation from interrupting an active scan
- Updated website positioning, product presentation, and pricing information

### Free and PRO

**Free** includes the core WiFi and network diagnostic experience.

**PRO** is a one-time upgrade that unlocks advanced LAN scanning capabilities, including enhanced scan controls such as configurable concurrency and subnet selection.

The app remains useful without PRO; the upgrade is focused on users who need deeper local-network visibility and more control over scanning.

---

## English

### Overview

**WiFi Health Check** is a focused local-network diagnostic app for iPhone and iPad.

It helps you understand whether a connectivity or local-network problem is related to:

- Public internet reachability
- DNS behavior
- Current WiFi connection
- WiFi security type
- Local gateway context
- LAN devices and services
- NAS, printers, access points, Proxmox hosts, servers, containers, and other infrastructure
- TCP connection stability
- WiFi roaming behavior
- Bonjour / mDNS advertised services
- Reachable TCP ports on local devices

The app is designed for foreground diagnosis and local visibility. It is not a background monitoring service, packet-capture tool, vulnerability scanner, or replacement for a full infrastructure monitoring platform.

### Key Features

| Capability | Description |
| --- | --- |
| One-tap network diagnostic | Review connectivity, DNS behavior, local IP, WiFi security context, gateway information, and diagnostic summary. |
| LAN device discovery | Discover devices available on the local network and review basic host information. |
| Port scanning | Check selected local devices for reachable TCP ports and common services. |
| Device & service identification | Use local signals and service fingerprints to better identify common infrastructure and software. |
| LAN TCP stability test | Test selected local services using custom TCP ports and repeated samples. |
| Bonjour / mDNS discovery | Discover local services advertised through standard Bonjour / mDNS protocols. |
| WiFi roaming report | Record SSID and BSSID samples while moving between WiFi coverage areas. |
| Privacy-first diagnostics | No account required; scan and diagnostic data is processed locally on the device. |

### LAN Scan

LAN Scan helps you discover devices on the local network and understand what is currently reachable.

Typical use cases include:

- Home routers and access points
- NAS devices
- Home servers
- Proxmox hosts
- Printers
- Smart-home / IoT devices
- Containers and self-hosted services
- Other local infrastructure

Advanced scan controls available through PRO are designed for users who need more flexibility when scanning larger or differently segmented local networks.

### Port Scanner

The Port Scanner helps determine which TCP services are reachable on a selected local device.

It is intended for:

- Troubleshooting local services
- Confirming expected ports are reachable
- Understanding what a device is exposing on the LAN
- Identifying common self-hosted and infrastructure services

It is a network diagnostic feature, not a vulnerability scanner.

### Device and Service Identification

WiFi Health Check combines network information, common ports, Bonjour / mDNS signals, and service fingerprints to improve local device identification.

The identification library covers common categories such as:

- NAS software
- Media services
- Windows and Windows Server
- Linux
- MySQL
- PostgreSQL
- Microsoft SQL Server
- DB2
- Other SQL services
- Portainer
- Kubernetes
- Bonjour / mDNS services

Identification is best-effort and may vary depending on how much information a device exposes on the local network.

### Bonjour / mDNS Service Discovery

WiFi Health Check can discover local services advertised through standard Bonjour / mDNS protocols.

This improves local-network visibility for services such as:

- NAS services
- Printers
- Web management interfaces
- Home servers
- Media services
- Other Bonjour-enabled applications and devices

This feature is designed for service visibility and discovery. It does not retrieve passwords, credentials, or private content.

### Built for Your Network

WiFi Health Check is designed for several common environments:

**Home Network**  
Quickly discover connected devices and troubleshoot common WiFi and LAN issues.

**NAS & Servers**  
Check local services, reachable ports, and common infrastructure running on your network.

**Smart Home**  
Find IoT devices and understand which services are visible on the LAN.

**Homelab**  
Inspect servers, containers, self-hosted services, Proxmox hosts, NAS systems, and other lab infrastructure from a mobile device.

---

## 简体中文

### 产品介绍

**WiFi Health Check** 是一款面向 iPhone 与 iPad 的本地 WiFi 与局域网诊断工具。

它可以帮助用户分析：

- 公网连通性
- DNS 行为
- 当前 WiFi 网络
- WiFi 安全类型
- 本地网关
- 局域网设备与服务
- NAS、打印机、AP、Proxmox 主机、服务器与容器
- TCP 稳定性
- WiFi 漫游行为
- Bonjour / mDNS 局域网服务
- 本地设备可访问的 TCP 端口

应用主要用于前台诊断和局域网可见性分析，不是后台持续监控服务、抓包工具、漏洞扫描器，也不是完整基础设施监控平台的替代品。

### v1.5 新增

- 增强 LAN Scan 局域网设备发现能力
- 新增 Port Scanner 端口扫描
- 支持可配置扫描并发
- 支持子网掩码选择
- 扩展设备与服务指纹识别库
- 加强 NAS、媒体服务、Windows / Windows Server、Linux、数据库、Portainer、Kubernetes 与 Bonjour 服务识别
- 新增统一的 PRO 高级扫描能力
- 扫描进行中限制可能导致扫描中断的页面切换
- 更新网站产品定位、功能展示与价格说明

### Free / PRO

**Free** 提供核心 WiFi 与网络诊断能力。

**PRO** 为一次性升级，主要解锁更高级的 LAN Scan 控制能力，包括扫描并发与子网选择等功能。

免费版本仍可完成基础诊断；PRO 面向需要更深入局域网可见性和扫描控制的用户。

### LAN Scan

LAN Scan 用于发现当前局域网内可访问的设备，并帮助理解本地网络中的设备分布。

适用于：

- 家庭路由器与 AP
- NAS
- 家庭服务器
- Proxmox 主机
- 打印机
- 智能家居 / IoT
- 容器与自托管服务
- 其他局域网基础设施

### Port Scanner

Port Scanner 用于检查指定局域网设备上可访问的 TCP 端口与常见服务。

适用于：

- 排查本地服务连接问题
- 确认预期端口是否可访问
- 了解设备在局域网内开放的服务
- 辅助识别自托管与基础设施服务

它用于网络诊断，不是漏洞扫描工具。

### 设备与服务识别

WiFi Health Check 会结合网络信息、常见端口、Bonjour / mDNS 信号和服务指纹，对本地设备进行尽可能准确的识别。

当前识别范围包括：

- NAS 软件
- 媒体服务
- Windows / Windows Server
- Linux
- MySQL
- PostgreSQL
- Microsoft SQL Server
- DB2
- 其他 SQL 服务
- Portainer
- Kubernetes
- Bonjour / mDNS 服务

识别结果属于 best-effort，实际效果取决于目标设备在局域网中公开的信息。

### Bonjour / mDNS 服务发现

通过标准 Bonjour / mDNS 协议发现局域网内公开服务。

适用于：

- NAS 服务
- 打印机
- Web 管理界面
- 家庭服务器
- 媒体服务
- 其他支持 Bonjour 的应用与设备

该功能用于服务可见性分析，不会读取账号密码、凭据或设备中的私有内容。

### 典型场景

**家庭网络**  
快速发现联网设备，并排查常见 WiFi 与局域网问题。

**NAS 与服务器**  
检查本地服务、开放端口以及常见基础设施。

**智能家居**  
发现 IoT 设备并了解其在局域网内公开的服务。

**Homelab**  
从手机或平板查看服务器、容器、自托管服务、Proxmox、NAS 等本地基础设施。



---

## Privacy

WiFi Health Check follows a privacy-first diagnostic model.

- No account required
- Network scans and diagnostics run locally on the device
- No diagnostic or LAN scan results are uploaded as part of normal app operation
- Reports remain on the device unless explicitly shared by the user
- App Store purchase / entitlement handling is separate from local diagnostic data

See the website privacy page for the current published policy.

---

## App Store

https://apps.apple.com/us/app/wifi-healthcheck/id6791147190

## Website

https://wifi.opshome.run

---

© 2026 OpsHome™. All rights reserved.
