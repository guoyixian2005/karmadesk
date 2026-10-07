# HANDOFF — Project06_数字疗愈解压工具 (KarmaDesk)

> 最后更新：2026-10-07 | 更新人：Gemini Spark (产品经理角色) | 交接给：人类 / 运维运营团队
> 规则：本文件是项目的「唯一事实来源」，**接手者必须先读本文件**。

## 1. 项目一句话概述

面向欧美年轻远程办公者与创作者的“3D对开推窗 · 灵签律动”微声疗与显化避难所（KarmaDesk v12.0 灵感签弹窗与氛围副屏屏保版），已完成全量产品调优与本地 Git 提交。

## 2. 技术栈 / 环境

- **前端技术栈**：HTML5 + Tailwind CSS + 原生 JavaScript + Web Audio API（136.1Hz 真实厚重铜钵声波 + 矿物敲击溪石 + 四音微风风铃 + 2.5s 平滑雨声）+ 3D 对开推窗视差系统
- **布局重构**：顶部三栏均衡布局，将 Karma 计数器移至左侧品牌区，彻底消除对中央小雅匾的视觉遮挡；
- **今日灵签（Daily Oracle）升级**：
  1. **每日首次访问自动弹出**：基于 `localStorage.karmadesk_last_oracle_date` 机制，每天第一次打开网站时自动柔和呈现当日宇宙箴言卡片；
  2. **流体毛玻璃质感重构**：背板升级为半透明悬浮遮罩（`backdrop-blur-md bg-black/35`），不再遮断窗外雨景与禅意桌面；弹窗卡片扩充至 `max-w-lg`，采用流体琥珀毛玻璃与微光金边质感，附带右上角关闭与一键同步至匾额按钮。
- **环境副屏屏保模式（Screensaver Focus Mode）重构**：
  1. **告别纯黑死寂**：去除原先沉闷的纯黑全屏遮挡，转为保留窗外 3D 推窗、动态山林雾气、丝雨飞落与红木桌案的半透明景深氛围屏保（`bg-black/35 backdrop-blur-[2px]`）；
  2. **优雅副屏时钟与日期**：大字号精致等宽数字时钟与优雅衬线英文日期显示；
  3. **4-7-8 呼吸脉动光晕与指示**：内置 19 秒完整循环的呼吸指引与微光膨胀收缩光晕（吸气 4s · 屏息 7s · 呼气 8s），助眠解压；
  4. **灵感禅语轮播**：内置多句优美英文禅意哲理语句，每隔 11 秒平滑淡入淡出轮换；
  5. **键盘触觉敲击依然生效**：副屏状态下按 `1`, `2`, `3`, `4`, `Space` 仍可敲击发声积攒 Karma，敲击时时钟产生柔和金色微光缩放反馈，随时敲击减压。
- **界面语言**：100% 地道纯正英文（零中文字符），海外直连。
- **交付形态**：纯静态单文件 Web 应用（直接双击 `index.html` 即可运行），零后端服务器维护成本，支持一键部署至 Vercel / Cloudflare Pages。
- **线上域名**：`https://karmadesk.comilla.world` / `https://karmadesk.vercel.app`。

## 3. 当前状态

阶段：**v12.0 灵感签弹窗与氛围副屏屏保完成，本地已提交，准备推送到 GitHub 触发 Vercel 自动部署** (100%)。

## 4. 关键文件索引

| 路径 | 说明 |
| :--- | :--- |
| [index.html](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/index.html) | v12.0 灵感签弹窗与氛围副屏屏保完整单页应用（直接双击浏览器秒开） |
| [docs/02_海外上线与部署运维SOP.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/02_海外上线与部署运维SOP.md) | GitHub 推送、Vercel 上线与 Gumroad 详细实操步骤 |
| [docs/01_产品需求文档_PRD.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/01_产品需求文档_PRD.md) | 完整 PRD 规范（功能、音效模型、定价与获客） |
| [docs/00_备选出海方向储备池.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/00_备选出海方向储备池.md) | 储备方向 A（社交凭证生成器）与 B（文字转卡片）备忘 |
| [HANDOFF.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/HANDOFF.md) | 项目唯一事实来源与执行断点 |
