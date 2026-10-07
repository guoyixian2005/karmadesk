# HANDOFF — Project06_数字疗愈解压工具 (KarmaDesk)

> 最后更新：2026-10-07 | 更新人：Gemini Spark (产品经理角色) | 交接给：人类 / 运维运营团队
> 规则：本文件是项目的「唯一事实来源」，**接手者必须先读本文件**。

## 1. 项目一句话概述

面向欧美年轻远程办公者与创作者的“3D对开推窗 · 灵签律动”微声疗与显化避难所（KarmaDesk v14.0 商业化收银台与高级副屏完备版），已完成全量产品调优与本地 Git 提交。

## 2. 技术栈 / 环境

- **前端技术栈**：HTML5 + Tailwind CSS + 原生 JavaScript + Web Audio API（136.1Hz 真实厚重铜钵声波 + 矿物敲击溪石 + 四音微风风铃 + 2.5s 平滑雨声）+ 3D 对开推窗视差系统
- **商业化收银台 (Monetization & Checkout)**：
  1. **顶部与底部 Pro 入口**：顶部导航新增金光微动的 `✨ Pro` 按钮，页脚新增 `✨ Pro ($4.99)` 升级入口；
  2. **典藏版弹窗 (KarmaDesk Pro Modal)**：包含 4 大高阶声景（京都古寺夜雪、夏夜深林雷雨、竹海松风、深海潮汐）、PWA 独立桌面版无边框运行、金匾专属刻字特权介绍；
  3. **集成 Gumroad 原生内嵌收银**：引入 `gumroad.js` 支持无缝页内滑出收银台（支持 Apple Pay / Google Pay / Visa / PayPal），无需跳离网页；
  4. **License Key 兑换与激活机制**：已购用户直接输入卡密激活 Pro 特权，本地状态即刻持久化。
- **环境副屏屏保模式（Screensaver Focus Mode）**：
  1. **背景彻底极简净化**：屏保触发时，桌上的铜钵、水晶、溪石、风铃与输入框自动 0.7s 优雅淡出淡化，背景**仅纯粹保留 3D 透视推窗、远山晨雾、翠竹露珠与实时细雨**；
  2. **高级制表级数字时钟（Horology Digital Clock）**：超细等宽数字，时分（`22:10`）与金色秒数角标（`37 SEC`）分层呈现，带金色柔光投影；
  3. **4-7-8 呼吸光晕与动态律动进度条**：内置完整 19 秒呼吸节律（吸气 4s · 屏息 7s · 呼气 8s），包含实时倒计时、呼吸状态文字、呼吸光晕与动态发光进度条；
  4. **典藏级禅意箴言卡**：微光黑金毛玻璃卡片搭配四角金纹装饰，精选英文哲思金句每隔 12 秒平滑淡入淡出轮换；
  5. **副屏快捷雨声与退出控制**：顶部悬浮集成雨声状态按钮与优雅退出标签；
  6. **键盘声学敲击互动**：副屏状态下按 `1`, `2`, `3`, `4`, `Space` 仍可直接敲击发声积攒 Karma，且敲击时呼吸光晕与时钟产生金色脉动微缩放反馈。
- **界面语言**：100% 地道纯正英文（零中文字符），海外直连。
- **交付形态**：纯静态单文件 Web 应用（直接双击 `index.html` 即可运行），零后端服务器维护成本，支持一键部署至 Vercel / Cloudflare Pages。
- **线上域名**：`https://karmadesk.comilla.world` / `https://karmadesk.vercel.app`。

## 3. 当前状态

阶段：**v14.0 商业化收银台与高级副屏完备版完成，本地已提交，准备推送到 GitHub 触发 Vercel 自动部署** (100%)。

## 4. 关键文件索引

| 路径 | 说明 |
| :--- | :--- |
| [index.html](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/index.html) | v14.0 商业化收银台与高级副屏完备版完整单页应用（直接双击浏览器秒开） |
| [docs/02_海外上线与部署运维SOP.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/02_海外上线与部署运维SOP.md) | GitHub 推送、Vercel 上线与 Gumroad 详细实操步骤 |
| [docs/01_产品需求文档_PRD.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/01_产品需求文档_PRD.md) | 完整 PRD 规范（功能、音效模型、定价与获客） |
| [docs/00_备选出海方向储备池.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/00_备选出海方向储备池.md) | 储备方向 A（社交凭证生成器）与 B（文字转卡片）备忘 |
| [HANDOFF.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/HANDOFF.md) | 项目唯一事实来源与执行断点 |
