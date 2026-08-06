<div align="center">

<img src="/docs/assets/images/app-logo.png" alt="WiFi Health Check Logo" width="120">

# WiFi Health Check

**Diagnose WiFi Problems from Your iPhone**  
**用 iPhone 快速诊断 WiFi 问题**

A privacy-first iPhone app for local WiFi and LAN diagnostics, including public internet reachability, WiFi security context, gateway information, TCP stability, and roaming behavior.

一款隐私优先的 iPhone 本地 WiFi 与局域网诊断应用，用于检查公网连通性、WiFi 安全类型、网关信息、TCP 稳定性和漫游行为。

<br>

[![App Store](https://img.shields.io/badge/App_Store-Download-0D96F6?logo=apple&logoColor=white)](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)
[![Website](https://img.shields.io/badge/Website-wifi.opshome.run-2EA866)](https://wifi.opshome.run)
[![Platform](https://img.shields.io/badge/Platform-iPhone-lightgrey?logo=apple)](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)
[![Privacy](https://img.shields.io/badge/Diagnostics-Local_Only-success)](https://wifi.opshome.run/privacy/)
[![Account](https://img.shields.io/badge/Account-Not_Required-blue)](https://wifi.opshome.run)

<br>

<a href="https://apps.apple.com/us/app/wifi-healthcheck/id6791147190">
  <img src="https://img.shields.io/badge/Download_on_the-App_Store-000000?logo=apple&logoColor=white&style=for-the-badge" alt="Download WiFi Health Check on the App Store">
</a>

<br><br>

<img src="/docs/assets/images/IMG_0540-portrait.png" alt="WiFi Health Check iPhone app showing current network and diagnostic status" width="300">

<br>

[English](#english) · [简体中文](#简体中文) · [Website](https://wifi.opshome.run) · [Privacy](https://wifi.opshome.run/privacy/) · [Support](https://wifi.opshome.run/support/) · [App Store](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)

</div>

---

## English

### Overview

**WiFi Health Check** is a focused iPhone app for quick, foreground WiFi and LAN troubleshooting.

It helps you understand whether a connection problem is related to:

- Public internet reachability
- DNS behavior
- The current WiFi network
- WiFi security type
- Local gateway context
- A router, NAS, printer, access point, Proxmox host, or server
- TCP connection stability
- WiFi roaming between access points

The app is designed for front-of-device diagnosis. It is not a background monitoring service, packet capture tool, or long-term infrastructure monitoring platform.

### Key Features

| Capability | Description |
| --- | --- |
| **One-tap network diagnostic** | Review public website connectivity, DNS behavior, local IP, WiFi security type, gateway address, and gateway TCP probe context in one report. |
| **LAN TCP stability test** | Test a router, NAS, printer, Proxmox host, access-point management address, or another LAN service using a custom TCP port and repeated samples. |
| **WiFi roaming report** | Record SSID and BSSID samples while moving and review the path between WiFi nodes. |
| **WiFi security context** | Display the current security type when iOS provides it, including Open, WEP, Personal, and Enterprise networks. |
| **Gateway information** | Show the estimated gateway address as supporting diagnostic context. |
| **Shareable text reports** | Save diagnostic, stability, and roaming results locally and share a clean text report when needed. |
| **No account required** | Run the app without registration or sign-in. |
| **No diagnostic cloud upload** | Reports remain on the iPhone unless you explicitly share them through iOS. |

### One-Tap Network Diagnostic

The main diagnostic report brings together several signals:

- Public website reachability
- DNS behavior
- Local IP address
- Estimated gateway address
- Gateway TCP probe context
- Current WiFi SSID
- Current WiFi BSSID when available
- WiFi security type when available
- Overall diagnostic summary

Public website reachability is treated as the primary internet connectivity signal. A closed gateway TCP port does not automatically mean that the internet connection is unavailable.

### LAN TCP Stability Test

Use the LAN TCP stability test when you need to check whether a specific local device or service remains reachable.

Example targets include:

- Router management interface
- NAS service
- Network printer
- Proxmox host
- Access-point management interface
- Home server
- Local web service
- Other devices using a known TCP port

Enter the target IP address and the correct TCP port. The app performs repeated samples so you can review connectivity, latency, and timeout behavior.

This test checks the selected TCP endpoint. It does not scan the full local network or discover passwords and credentials.

### WiFi Roaming Report

The roaming report helps you observe how an iPhone moves between WiFi nodes.

While walking through a home or office:

1. Keep WiFi Health Check in the foreground.
2. Start a roaming test.
3. Move between rooms or access-point coverage areas.
4. Review the SSID and BSSID sample sequence.
5. Compare when the device stayed on one node or moved to another.

The report is useful when investigating sticky-client behavior, uneven access-point coverage, or unexpected roaming paths.

### WiFi Security Context

When iOS provides the information, WiFi Health Check can display the current WiFi security type, including:

- Open
- WEP
- Personal
- Enterprise

WiFi security information is diagnostic context. Availability depends on iOS permissions, entitlements, the current connection, and system privacy behavior.

### How It Works

1. **Connect a real iPhone to WiFi**  
   Use the app on a physical iPhone connected to a WiFi network.

2. **Allow Location permission when needed**  
   iOS requires Location permission before ordinary App Store apps can access current-network details such as SSID, BSSID, and security type.

3. **Choose a focused test**  
   Run the one-tap diagnostic, LAN TCP stability test, or WiFi roaming report.

4. **Review the local result**  
   Compare internet reachability, DNS, gateway context, TCP samples, timeouts, and roaming changes.

5. **Share only when needed**  
   Reports remain on the device unless you explicitly use the iOS sharing interface.

### Understanding the Results

WiFi problems can originate from different parts of the connection path:

| Area | Example issue | Useful signal |
| --- | --- | --- |
| **Internet** | Broadband or upstream connectivity problem | Public website reachability |
| **DNS** | Domain resolution failure or delay | DNS behavior |
| **Gateway** | Local routing or gateway configuration context | Gateway address and supporting TCP probe |
| **LAN device** | NAS, printer, server, AP, or router service instability | Custom TCP stability samples |
| **WiFi security** | Unexpected open, legacy, personal, or enterprise network context | Current security type |
| **Roaming** | iPhone remains connected to the wrong WiFi node | SSID and BSSID sequence |

The app separates these signals into smaller reports so that they can be compared across rooms, devices, and networks.

### Privacy-First Design

WiFi Health Check is designed as a local foreground diagnostic app.

The app may process the following information locally on the iPhone:

- Current WiFi SSID
- Current WiFi BSSID when provided by iOS
- WiFi security type when provided by iOS
- Local IP address
- Estimated gateway address
- Public website connectivity results
- Custom LAN target IP address and TCP port entered by the user
- Diagnostic history
- TCP stability samples
- WiFi roaming samples
- Language preference
- Saved local reports

WiFi Health Check does not require account registration and does not upload diagnostic history to an OpsHome cloud service. Reports leave the device only when the user explicitly shares them through iOS.

The app does not collect:

- Router passwords
- WiFi passwords
- Packet capture data
- Browsing history
- Account identity for app registration
- RSSI, channel, frequency band, channel width, or PHY rate that ordinary App Store apps cannot reliably obtain from iOS

Read the complete [Privacy Policy](https://wifi.opshome.run/privacy/).

### Why Location Permission Is Needed

iOS restricts access to current WiFi details such as SSID, BSSID, and security type.

WiFi Health Check uses Location permission only to request the current-network information that iOS permits. The app does not need the user's physical location history for WiFi diagnosis.

If SSID, BSSID, or security type is unavailable, check that:

- You are using a physical iPhone
- The iPhone is connected to WiFi
- The app is not running in Simulator
- Location permission has been allowed
- iOS is currently providing the requested network details

### iOS WiFi Information Limitations

Ordinary App Store apps do not receive reliable access to several low-level WiFi measurements, including:

- RSSI
- WiFi channel
- Frequency band
- Channel width
- PHY rate

WiFi Health Check therefore focuses on information and behavior that iOS permits, such as:

- Public connectivity
- DNS behavior
- TCP connectivity
- Latency
- Timeouts
- Current WiFi identifiers
- Security context
- Roaming behavior

### What WiFi Health Check Is Not

WiFi Health Check is not:

- A packet-capture or traffic-inspection tool
- A WiFi password recovery tool
- A router administration client
- A full LAN vulnerability scanner
- A background uptime-monitoring platform
- A replacement for professional WiFi survey hardware
- A source of RSSI, channel, band, or PHY-rate data unavailable through normal iOS APIs

### Need Continuous Infrastructure Monitoring?

WiFi Health Check is designed for local foreground diagnosis.

For continuous monitoring, alerts, history, Docker Probe, Synology NAS, Proxmox VE, Linux hosts, Docker containers, websites, and private services, use **OpsHome NOC**.

[Learn about OpsHome NOC](https://app.opshome.run) · [Visit OpsHome](https://opshome.run)

### App Availability

WiFi Health Check is available on the App Store for iPhone.

[Download WiFi Health Check on the App Store](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)

### Support

For product support:

- Visit the [WiFi Health Check Support page](https://wifi.opshome.run/support/)
- Include the app version
- Include the iOS version
- Include the iPhone model
- Describe the problem and the test being used
- Do not send WiFi passwords, router administrator passwords, or private credentials

---

## 简体中文

### 产品介绍

**WiFi Health Check** 是一款面向 iPhone 的本地 WiFi 和局域网快速排障工具。

它可以帮助用户判断连接问题是否与以下因素有关：

- 公网连通性
- DNS 行为
- 当前 WiFi 网络
- WiFi 安全类型
- 本地网关
- 路由器、NAS、打印机、AP、Proxmox 主机或服务器
- TCP 连接稳定性
- 多个接入点之间的 WiFi 漫游

这是一款前台本地诊断工具，不是后台持续监控服务、抓包工具或完整的基础设施监控平台。

### 核心功能

| 功能 | 说明 |
| --- | --- |
| **一键网络诊断** | 在一份报告中检查公网网站连通性、DNS 行为、本机 IP、WiFi 安全类型、网关地址和网关 TCP 探测上下文。 |
| **LAN TCP 稳定性测试** | 使用自定义 TCP 端口，对路由器、NAS、打印机、Proxmox 主机、AP 管理地址或其他局域网服务进行连续采样。 |
| **WiFi 漫游报告** | 移动过程中记录 SSID 和 BSSID 样本，查看 iPhone 在不同 WiFi 节点之间的连接路径。 |
| **WiFi 安全类型** | 当 iOS 提供时，显示开放、WEP、个人和企业网络等当前安全类型。 |
| **网关信息** | 显示估算的当前网关地址，作为诊断辅助信息。 |
| **可分享文本报告** | 将诊断、稳定性和漫游结果保存在本机，需要时再分享清晰的文本报告。 |
| **无需账号** | 无需注册或登录即可使用。 |
| **不上传诊断历史** | 报告保留在 iPhone 上，只有用户主动通过 iOS 分享时才会离开设备。 |

### 一键网络诊断

主诊断报告会集中显示多项信号：

- 公网网站连通性
- DNS 行为
- 本机 IP 地址
- 估算的网关地址
- 网关 TCP 探测上下文
- 当前 WiFi SSID
- iOS 可提供时的当前 BSSID
- iOS 可提供时的 WiFi 安全类型
- 总体诊断摘要

公网网站连通性是判断互联网状态的主要信号。网关某个 TCP 端口关闭，并不等于互联网连接已经中断。

### LAN TCP 稳定性测试

当需要检查某个局域网设备或服务是否持续可达时，可以使用 LAN TCP 稳定性测试。

适合测试的目标包括：

- 路由器管理界面
- NAS 服务
- 网络打印机
- Proxmox 主机
- AP 管理界面
- 家庭服务器
- 局域网 Web 服务
- 其他使用已知 TCP 端口的设备

输入目标 IP 地址和正确的 TCP 端口后，应用会执行连续采样，帮助查看连通性、延迟和超时情况。

该测试只检查指定的 TCP 端点，不会扫描整个局域网，也不会获取密码或凭据。

### WiFi 漫游报告

漫游报告用于观察 iPhone 在不同 WiFi 节点之间的切换行为。

测试方式：

1. 保持 WiFi Health Check 在前台运行。
2. 启动漫游测试。
3. 在房间或不同 AP 覆盖区域之间移动。
4. 查看 SSID 和 BSSID 的采样序列。
5. 判断设备何时停留在原节点，以及何时切换到另一个节点。

该报告适合调查客户端黏连、AP 覆盖不均和异常漫游路径等问题。

### WiFi 安全类型

当 iOS 提供相关信息时，应用可以显示：

- Open
- WEP
- Personal
- Enterprise

WiFi 安全类型仅作为诊断上下文。能否获得该信息取决于 iOS 权限、应用能力、当前连接和系统隐私限制。

### 工作方式

1. **使用真实 iPhone 连接 WiFi**  
   请在已连接 WiFi 的实体 iPhone 上运行应用。

2. **需要时允许位置权限**  
   iOS 要求普通 App Store 应用获得位置权限后，才能请求 SSID、BSSID 和安全类型等当前网络信息。

3. **选择适合的测试**  
   根据问题运行一键诊断、LAN TCP 稳定性测试或 WiFi 漫游报告。

4. **查看本地结果**  
   对比公网连通性、DNS、网关上下文、TCP 样本、超时和漫游变化。

5. **需要时再分享**  
   报告默认留在设备上，只有用户主动使用 iOS 分享功能时才会离开设备。

### 如何理解检测结果

WiFi 问题可能来自连接路径中的不同位置：

| 范围 | 问题示例 | 可参考的信号 |
| --- | --- | --- |
| **互联网** | 宽带或上游连接异常 | 公网网站连通性 |
| **DNS** | 域名解析失败或延迟 | DNS 行为 |
| **网关** | 本地路由或网关配置问题 | 网关地址和辅助 TCP 探测 |
| **局域网设备** | NAS、打印机、服务器、AP 或路由器服务不稳定 | 自定义 TCP 连续采样 |
| **WiFi 安全** | 连接到了意外的开放、旧式、个人或企业网络 | 当前安全类型 |
| **漫游** | iPhone 长时间停留在错误的 WiFi 节点 | SSID 和 BSSID 序列 |

应用会将这些信号拆分成多个小报告，便于比较不同房间、设备和网络环境中的结果。

### 隐私优先设计

WiFi Health Check 是一款本地前台诊断应用。

应用可能在 iPhone 本机处理：

- 当前 WiFi SSID
- iOS 可提供时的当前 BSSID
- iOS 可提供时的 WiFi 安全类型
- 本机 IP 地址
- 估算的网关地址
- 公网网站连通性结果
- 用户输入的 LAN 目标 IP 地址和 TCP 端口
- 诊断历史
- TCP 稳定性样本
- WiFi 漫游样本
- 语言偏好
- 本地保存的报告

WiFi Health Check 不要求注册账号，也不会将诊断历史上传到 OpsHome 云端服务。只有用户主动通过 iOS 分享时，报告才会离开设备。

应用不会收集：

- 路由器密码
- WiFi 密码
- 抓包数据
- 浏览历史
- 用于应用注册的账号身份
- 普通 App Store 应用无法从 iOS 可靠获得的 RSSI、信道、频段、信道宽度或 PHY 速率

查看完整的[隐私政策](https://wifi.opshome.run/privacy/)。

### 为什么需要位置权限

iOS 限制普通应用读取 SSID、BSSID 和 WiFi 安全类型等当前网络信息。

WiFi Health Check 只使用位置权限请求 iOS 允许提供的当前网络信息，不需要用户的实际位置历史来完成 WiFi 诊断。

SSID、BSSID 或安全类型不可用时，请确认：

- 正在使用实体 iPhone
- iPhone 已连接 WiFi
- 没有使用 Simulator
- 已允许位置权限
- iOS 当前允许返回对应的网络信息

### iOS WiFi 信息限制

普通 App Store 应用无法可靠读取以下底层 WiFi 参数：

- RSSI
- WiFi 信道
- 频段
- 信道宽度
- PHY 速率

因此，WiFi Health Check 主要使用 iOS 允许访问的信息与行为进行诊断，包括：

- 公网连通性
- DNS 行为
- TCP 连通性
- 延迟
- 超时
- 当前 WiFi 标识
- 安全类型
- 漫游行为

### WiFi Health Check 不是什么

WiFi Health Check 不是：

- 抓包或流量分析工具
- WiFi 密码恢复工具
- 路由器管理客户端
- 完整的局域网漏洞扫描器
- 后台持续运行的可用性监控平台
- 专业 WiFi 勘测硬件的替代品
- 普通 iOS API 无法提供的 RSSI、信道、频段或 PHY 速率来源

### 需要持续基础设施监控？

WiFi Health Check 用于本地前台诊断。

如需持续监控、告警、历史记录、Docker Probe、Synology NAS、Proxmox VE、Linux 主机、Docker 容器、网站和私有服务，请使用 **OpsHome NOC**。

[了解 OpsHome NOC](https://app.opshome.run) · [访问 OpsHome](https://opshome.run)

### App Store

WiFi Health Check 已在 App Store 上架，面向 iPhone 提供。

[在 App Store 下载 WiFi Health Check](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)

### 支持

需要产品支持时：

- 访问 [WiFi Health Check 支持页面](https://wifi.opshome.run/support/)
- 提供应用版本
- 提供 iOS 版本
- 提供 iPhone 型号
- 简要说明问题以及正在使用的测试
- 请勿发送 WiFi 密码、路由器管理员密码或其他私有凭据

---

**Free. Local-only. Built for quick troubleshooting.**  
**免费。本地优先。为快速排障而设计。**

[Website](https://wifi.opshome.run) · [App Store](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190) · [Privacy](https://wifi.opshome.run/privacy/) · [Support](https://wifi.opshome.run/support/)

<br>

© 2026 OpsHome™. All rights reserved.

</div>
