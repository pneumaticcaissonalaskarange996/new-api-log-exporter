# New API 使用日志导出 / Usage Log Exporter

> Chrome 浏览器扩展 — 为 New API / One API 控制台添加一键导出账单 CSV 功能

[![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-blue?logo=googlechrome)](https://github.com/jiusimeng8-cmd/new-api-log-exporter)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 这是什么？ / What is this?

一个轻量 Chrome 扩展，为 [New API](https://github.com/Calcium-Ion/new-api)（及 [One API](https://github.com/songquanpeng/one-api)）的  使用日志页面增加 **导出账单** 按钮，一键将所有 API 调用记录导出为 CSV 文件，方便对账、报销、成本分析。

A lightweight Chrome extension that adds an **Export Bill** button to the usage log page of any New API / One API deployment. Export all API call records to CSV with one click — perfect for billing reconciliation, expense reporting, and cost analysis.

## 能做什么？ / What can it do?

- 📊 **一键导出全部日志**为 CSV（Excel 直接打开）
- 🔍 **按条件筛选导出**：时间范围、令牌、分组、消费类型、模型
- 💰 **完整计费明细**：Token 用量、花费(USD)、渠道、分组倍率、模型倍率、Request ID
- 🌐 **通配任意 New API/One API 站点**，不限域名
- ⚡ **自动分页拉取**，上千条数据也能快速导出

---

- 📊 **One-click CSV export** (Excel-ready)
- 🔍 **Filter by**: date range, token name, group, type, model name
- 💰 **Full billing details**: token usage, cost (USD), channel, ratios, Request ID
- 🌐 **Universal**: works on any New API / One API deployment
- ⚡ **Auto-pagination**: fetches thousands of records efficiently

## 安装 / Install

1. 下载本仓库 ZIP 并解压，或 `git clone` 到本地
2. Chrome 打开 `chrome://extensions`
3. 右上角开启 **开发者模式**
4. 点击 **加载未打包的扩展程序**，选择本目录
5. 打开任意 New API 实例的 `/console/log` 页面，工具栏右侧出现 **导出账单** 按钮

---

1. Download and extract this repo, or `git clone`
2. Open `chrome://extensions` in Chrome
3. Enable **Developer mode** (top right)
4. Click **Load unpacked** and select this folder
5. Visit `/console/log` on any New API instance — an **导出账单** button appears

## 功能 / Features

- 点击按钮弹出配置窗口，可筛选：
  - 时间范围（默认当天）
  - 令牌名称、分组、类型（消费/充值/全部）、模型名称
- 导出为 UTF-8 CSV（Excel 直接打开不乱码）
- 包含完整的计费明细：Token 用量、花费(USD)、渠道、倍率、Request ID
- 自动分页拉取全部数据

---

- Click the button to open a filter dialog:
  - Date range (defaults to today)
  - Token name, Group, Type (consume/recharge/all), Model name
- Exports as UTF-8 CSV (BOM included, Excel-ready)
- Full billing details: token usage, cost (USD), channel, ratios, Request ID
- Automatically fetches all pages

## 兼容性 / Compatibility

匹配所有 New API 实例的 `/console/log*` 路径，不限于特定域名。

Works on any New API deployment — not tied to a specific domain.

## 开发声明 / Development Note

本项目从需求整理、代码实现、README、SEO 优化到发布 GitHub，全程由 AI 辅助完成。开发过程中使用了 [cli.999554.xyz](https://cli.999554.xyz)（云舟中转站）提供的 API 服务。这个项目本身就是 AI 开发工作流的产物。

This project was built end-to-end with AI assistance — from requirements, coding, README, SEO optimization, to GitHub release. API services used during development were provided by [cli.999554.xyz](https://cli.999554.xyz). The project itself is a product of an AI-driven development workflow.

## 许可 / License

MIT
