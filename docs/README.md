<div align="center">

<img src="/docs/assets/images/app-logo-96.webp" alt="WiFi Health Check Logo" width="120">


# WiFi Health Check

**Diagnose WiFi Problems from Your iPhone**\
**用 iPhone 快速诊断 WiFi 问题**

A privacy-first iPhone app for local WiFi and LAN diagnostics, including
public internet reachability, WiFi security context, gateway
information, TCP stability, roaming behavior, and Bonjour / mDNS local
service discovery.

一款隐私优先的 iPhone 本地 WiFi
与局域网诊断应用，用于检查公网连通性、WiFi 安全类型、网关信息、TCP
稳定性、漫游行为以及 Bonjour / mDNS 局域网服务发现。

`<br>`{=html}

[![App
Store](https://img.shields.io/badge/App_Store-Download-0D96F6?logo=apple&logoColor=white)](https://apps.apple.com/us/app/wifi-healthcheck/id6791147190)

[![Website](https://img.shields.io/badge/Website-wifi.opshome.run-2EA866)](https://wifi.opshome.run)

[![Privacy](https://img.shields.io/badge/Diagnostics-Local_Only-success)](https://wifi.opshome.run/privacy/)
:::

------------------------------------------------------------------------

## v1.4 Update

WiFi Health Check v1.4 introduces:

-   Bonjour / mDNS service discovery
-   Improved local network visibility
-   Better LAN service identification
-   Updated website presentation with additional screenshots
-   Improved multilingual product consistency

------------------------------------------------------------------------

# English

## Overview

**WiFi Health Check** is a focused iPhone app for quick WiFi and LAN
troubleshooting.

It helps you understand whether a connection problem is related to:

-   Public internet reachability
-   DNS behavior
-   Current WiFi network
-   WiFi security type
-   Local gateway
-   Router, NAS, printer, access point, Proxmox host, or server
-   TCP connection stability
-   WiFi roaming behavior
-   Local network services discovered through Bonjour / mDNS

The app is designed for foreground diagnosis. It is not a background
monitoring service, packet capture tool, or infrastructure monitoring
platform.

## Key Features

  -----------------------------------------------------------------------
  Capability                          Description
  ----------------------------------- -----------------------------------
  One-tap network diagnostic          Review connectivity, DNS behavior,
                                      local IP, WiFi security context,
                                      gateway information and diagnostic
                                      summary.

  LAN TCP stability test              Test selected local services using
                                      custom TCP ports and repeated
                                      samples.

  Bonjour / mDNS service discovery    Discover available local network
                                      services advertised through
                                      standard Bonjour / mDNS protocols.

  WiFi roaming report                 Record SSID and BSSID samples while
                                      moving between WiFi coverage areas.

  WiFi security context               Display current WiFi security type
                                      when iOS provides the information.

  Shareable reports                   Save diagnostic results locally and
                                      share when needed.

  No account required                 Use the app without registration or
                                      sign-in.

  No diagnostic cloud upload          Reports remain on the iPhone unless
                                      explicitly shared.
  -----------------------------------------------------------------------

## Bonjour / mDNS Service Discovery

WiFi Health Check v1.4 adds local service discovery based on Bonjour /
mDNS.

This helps identify services available inside the local network, such
as:

-   NAS services
-   Printers
-   Web management interfaces
-   Home servers
-   Other Bonjour-enabled services

The feature focuses on service visibility and discovery. It does not
perform vulnerability scanning or credential discovery.

------------------------------------------------------------------------

# 简体中文

## 产品介绍

**WiFi Health Check** 是一款面向 iPhone 的本地 WiFi
与局域网快速排障工具。

它可以帮助用户判断连接问题是否与以下因素有关：

-   公网连通性
-   DNS 行为
-   当前 WiFi 网络
-   WiFi 安全类型
-   本地网关
-   路由器、NAS、打印机、AP、Proxmox 主机或服务器
-   TCP 连接稳定性
-   WiFi 漫游行为
-   Bonjour / mDNS 局域网服务发现

这是一款前台诊断工具，不是后台持续监控服务、抓包工具或完整基础设施监控平台。

## v1.4 新增

-   新增 Bonjour / mDNS 服务发现
-   增强局域网服务可见性
-   改进 LAN 服务识别
-   更新产品截图展示
-   优化多语言页面一致性

## Bonjour / mDNS 服务发现

通过标准 Bonjour / mDNS 协议发现局域网内公开服务。

可辅助识别：

-   NAS 服务
-   打印机
-   Web 管理界面
-   家庭服务器
-   其他支持 Bonjour 的设备服务

该功能用于服务可见性分析，不是漏洞扫描工具，也不会获取账号密码。

------------------------------------------------------------------------

# Website Repository

This repository contains the static marketing, privacy, support, and
product information website for WiFi Health Check.

## Published Pages

  Path          Purpose
  ------------- -------------------------------------
  `/`           English product homepage
  `/zh-cn/`     Simplified Chinese product homepage
  `/privacy/`   Privacy policy
  `/support/`   Product support and troubleshooting
  `/about/`     Product and OpsHome background

## Website Assets

Current website assets include:

-   WiFi Status screenshot
-   LAN Scan and Bonjour / mDNS screenshot
-   App icons
-   Social sharing images
-   Website branding assets

Unused legacy images have been removed.

------------------------------------------------------------------------

# Privacy

WiFi Health Check follows a privacy-first design.

-   No account required
-   No diagnostic cloud upload
-   Reports stay locally on the device
-   Data leaves the device only when users explicitly share through iOS

------------------------------------------------------------------------

# App Store

https://apps.apple.com/us/app/wifi-healthcheck/id6791147190

# Website

https://wifi.opshome.run

------------------------------------------------------------------------

© 2026 OpsHome™. All rights reserved.
