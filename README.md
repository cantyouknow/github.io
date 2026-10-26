# cantyouknow.com — 个人站点

> 🌤️ 一个关于天气、心情与周期的小站。查天气、测心情、听心语，读康波，也卜一卦。

**在线访问**：<https://cantyouknow.com/>

## 技术栈

React + TypeScript + Vite + Tailwind CSS + shadcn/ui，构建为纯静态站点托管于 GitHub Pages（HashRouter）。源码在 `app/` 目录，构建产物（`index.html` + `assets/` + `data/` + `archives/`）部署于仓库根目录。

## 站点页面

| 页面 | 说明 |
|------|------|
| 🏠 [心情天气站](https://cantyouknow.com/#/) | 首页。城市天气查询 + 心情寄语，数据来自 Open-Meteo / 一言 API，含本地语库兜底 |
| 📊 [康波周期投资策略报告](https://cantyouknow.com/#/kangbo) | 基于周金涛康波周期理论的市场观察报告，**每月1日自动更新**（当前：2026年10月版），报告数据驱动（`data/report-current.json`），含历史版本切换 |
| 🔮 [小六壬卜卦](https://cantyouknow.com/#/liuren) | 默念所问之事，输入闪过的数字，掐指演算短期/中期/长期三层结果（国风古卷视觉） |
| 📜 [历史归档](https://cantyouknow.com/archives/) | 早期 HTML 版报告（2026年1月/2月版）永久留存 |

## 报告更新约定

- 每月1日 09:00 自动更新：取当月行情数据 → 复盘上月预测（✓对/✗错/◐半）→ 生成新 `data/report-current.json` → 旧版归档为 `data/report-YYYY-MM.json`
- 归档 JSON 一经生成永不修改；更早期 HTML 归档在 `archives/`
- 完整流程与红线见仓库外工作目录 `automation_prompt.md`

## 免责声明

站内投资相关内容仅供学习参考，不构成任何投资建议。市场有风险，投资需谨慎。小六壬为传统文化娱乐参考，心诚则灵，事在人为。
