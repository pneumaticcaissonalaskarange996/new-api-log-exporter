# New API 使用日志导出

> Chrome 浏览器扩展 — 为 New API / One API 控制台添加一键导出账单 CSV 功能

[![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-blue?logo=googlechrome)](https://github.com/jiusimeng8-cmd/new-api-log-exporter)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 这是什么？

一个轻量 Chrome 扩展，为 [New API](https://github.com/Calcium-Ion/new-api)（及 [One API](https://github.com/songquanpeng/one-api)）的使用日志页面增加 **导出账单** 按钮，一键将所有 API 调用记录导出为 CSV 文件，方便对账、报销、成本分析。

## 能做什么？

- 📊 **一键导出全部日志**为 CSV（Excel 直接打开，UTF-8 BOM 不乱码）
- 🔍 **按条件筛选导出**：时间范围、令牌名称、分组、消费类型、模型名称
- 💰 **完整计费明细**：Token 用量、花费(USD)、渠道、分组倍率、模型倍率、Request ID
- 🌐 **通配任意 New API / One API 站点**，不限于特定域名
- ⚡ **自动分页拉取**，上千条数据也能快速导出

## 安装

1. 下载本仓库 ZIP 并解压，或 `git clone` 到本地
2. Chrome 打开 `chrome://extensions`
3. 右上角开启 **开发者模式**
4. 点击 **加载未打包的扩展程序**，选择本目录
5. 打开任意 New API 实例的 `/console/log` 页面，工具栏右侧出现 **导出账单** 按钮

## 使用方式

点击「导出账单」按钮 → 弹出配置窗口：

| 筛选项 | 默认值 |
|--------|--------|
| 开始时间 | 当天 00:00 |
| 结束时间 | 当天 23:59 |
| 令牌名称 | 空（全部） |
| 分组 | 空（全部） |
| 类型 | 全部（可切换消费/充值） |
| 模型名称 | 空（全部） |

设置好筛选条件后点「导出 CSV」，等待进度条完成即可下载。

## 兼容性

匹配所有 New API / One API 实例的 `/console/log*` 路径，不限于特定域名。自动适配目标站点的 API 地址和额度换算。

## 开发声明

本项目从需求整理、代码实现、README、SEO 优化到发布 GitHub，全程由 AI 辅助完成。开发过程中使用了 [cli.999554.xyz](https://cli.999554.xyz)（云舟中转站）提供的 API 服务。这个项目本身就是 AI 开发工作流的产物。

## 许可

MIT

---

# New API Usage Log Exporter

> Chrome extension — adds one-click CSV bill export to any New API / One API console

## What is this?

A lightweight Chrome extension that adds an **Export Bill** button to the usage log page of any [New API](https://github.com/Calcium-Ion/new-api) or [One API](https://github.com/songquanpeng/one-api) deployment. Export all API call records to CSV with one click — perfect for billing reconciliation, expense reporting, and cost analysis.

## Features

- 📊 **One-click CSV export** (Excel-ready, UTF-8 BOM)
- 🔍 **Filter by**: date range, token name, group, type, model name
- 💰 **Full billing details**: token usage, cost (USD), channel, group ratio, model ratio, Request ID
- 🌐 **Universal**: works on any New API / One API deployment
- ⚡ **Auto-pagination**: efficiently fetches thousands of records

## Installation

1. Download the ZIP or `git clone` this repo
2. Open `chrome://extensions` in Chrome
3. Enable **Developer mode** (top right)
4. Click **Load unpacked** and select this folder
5. Visit `/console/log` on any New API instance — the **导出账单** button appears next to the filter toolbar

## Usage

Click **导出账单** → a filter dialog appears:

| Filter | Default |
|--------|---------|
| Start time | Today 00:00 |
| End time | Today 23:59 |
| Token name | Empty (all) |
| Group | Empty (all) |
| Type | All (consume / recharge) |
| Model name | Empty (all) |

Set your filters and click **导出 CSV**. Wait for the progress bar to complete, then your file downloads automatically.

## Compatibility

Matches `/console/log*` on any New API / One API instance — not tied to a specific domain. Automatically adapts to the target site's API base URL and quota conversion.

## Development Note

This project was built end-to-end with AI assistance — from requirements, coding, README, SEO optimization, to GitHub release. API services used during development were provided by [cli.999554.xyz](https://cli.999554.xyz). The project itself is a product of an AI-driven development workflow.

## License

MIT
