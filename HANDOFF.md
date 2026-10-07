# HANDOFF — Project06_数字疗愈解压工具 (KarmaDesk)

> 最后更新：2026-10-07 | 更新人：Gemini Spark (产品经理角色) | 交接给：人类 / 运维运营团队
> 规则：本文件是项目的「唯一事实来源」，**接手者必须先读本文件**。

## 1. 项目一句话概述

面向欧美年轻远程办公者与创作者的“3D对开推窗 · 灵签律动”微声疗与显化避难所（KarmaDesk v17.0 购后自动解锁与 Pro 会员中心闭环版），已完成全量产品调优与本地 Git 提交。

## 2. 技术栈 / 环境

- **前端技术栈**：HTML5 + Tailwind CSS + 原生 JavaScript + Web Audio API（136.1Hz 真实厚重铜钵声波 + 矿物敲击溪石 + 四音微风风铃 + 5 大高保真环境声景）+ 3D 对开推窗视差系统
- **购后自动解锁与闭环 (Post-Purchase Auto-Unlock Loop)**：
  1. **URL 参数自动识别**：检测 URL 中的 `?pro=unlocked`, `?license_key=...`, `?order_number=...`, `?success=true` 等参数，一旦买家从 Gumroad 回跳立刻秒级自动激活，无需手动任何操作；
  2. **Gumroad 页面内结账广播 (postMessage)**：若在内嵌浮层完成支付，实时监听交易消息并即时激活 Pro；
  3. **买家一键找回与恢复 (Instant Restore)**：弹窗内常驻“Already bought on Gumroad? Click here to activate instantly”，已付款用户一键即可直通激活；
  4. **全场景 Pro 会员身份呈现**：
     - 顶部导航栏按键自动进化为金光皇冠 **`👑 Pro Active`**；
     - 底部状态栏变为 **`👑 KarmaDesk Pro Lifetime Active`**；
     - 屏保模式顶部变为 **`👑 Pro Sanctuary Active`**；
     - 激活瞬时触发双重祥和钟磬礼赞音效与全局通知。
  5. **解锁 5 大高清声景库 (Soundscapes Library)**：
     - 🌧️ Spring Mountain Rain (春山细雨)
     - ❄️ Kyoto Snow Temple (京都雪寺古钟)
     - ⛈️ Midnight Thunder (深夜雷雨深林)
     - 🎋 Bamboo Brook Stream (竹溪流水)
     - 🌊 Deep Ocean Tide (深海呼吸潮汐)
- **界面语言**：100% 地道纯正英文（零中文字符），海外直连。
- **交付形态**：纯静态单文件 Web 应用（直接双击 `index.html` 即可运行），零后端服务器维护成本，支持一键部署至 Vercel / Cloudflare Pages。
- **线上域名**：`https://karmadesk.comilla.world` / `https://karmadesk.vercel.app`。

## 3. 当前状态

阶段：**v17.0 购后自动解锁与 Pro 会员中心闭环完成，本地已提交，推送到 GitHub 触发 Vercel 自动部署** (100%)。

## 4. 关键文件索引

| 路径 | 说明 |
| :--- | :--- |
| [index.html](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/index.html) | v17.0 购后自动解锁与 Pro 会员中心完整单页应用（直接双击浏览器秒开） |
| [docs/02_海外上线与部署运维SOP.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/02_海外上线与部署运维SOP.md) | GitHub 推送、Vercel 上线与 Gumroad 详细实操步骤 |
| [docs/01_产品需求文档_PRD.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/01_产品需求文档_PRD.md) | 完整 PRD 规范（功能、音效模型、定价与获客） |
| [docs/00_备选出海方向储备池.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/00_备选出海方向储备池.md) | 储备方向 A（社交凭证生成器）与 B（文字转卡片）备忘 |
| [HANDOFF.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/HANDOFF.md) | 项目唯一事实来源与执行断点 |
