# HANDOFF — Project06_数字疗愈解压工具 (KarmaDesk)

> 最后更新：2026-10-07 | 更新人：Gemini Spark (产品经理角色) | 交接给：人类 / 运维运营团队
> 规则：本文件是项目的「唯一事实来源」，**接手者必须先读本文件**。

## 1. 项目一句话概述

面向欧美年轻远程办公者与创作者的“3D对开推窗 · 纵深雨境”微声疗与显化避难所（KarmaDesk），已完成全量产品打磨与本地 Git 初始化提交，进入正式上线部署阶段。

## 2. 技术栈 / 环境

- **前端技术栈**：HTML5 + Tailwind CSS + 原生 JavaScript + Web Audio API（程序合成物理声学，含 2.5s 雨声平滑指数渐变）+ Canvas 2D 窗外三层景深细雨引擎 + CSS 3D 透视推窗系统
- **部署平台**：Vercel Serverless / Cloudflare Pages（零服务器运维成本，全球 Anycast CDN，自带免费 SSL）
- **代码仓库**：本地已初始化 Git 仓库并完成全量版本提交 (`master` 36cedd3)
- **收银通道**：Gumroad Checkout ($4.99 一次性买断)

## 3. 当前状态

阶段：**MVP 研发与体验调优 100% 完成，Git 仓库提交就绪，进入上线发布流程** (95%)。

## 4. 当前断点（从哪里继续）

- 本地交付物完备：
  1. `index.html`：生产就绪型单页纯静态应用（零后端、秒级加载、支持离线与 PWA）；
  2. `docs/01_产品需求文档_PRD.md`：完整需求规范、竞品真空、定价与 GTM 获客指南；
  3. `docs/02_海外上线与部署运维SOP.md`：详细记录 GitHub 推送、Vercel 部署、Gumroad 绑定的标准 SOP；
  4. `docs/00_备选出海方向储备池.md`：方向 A 与 B 的完整归档。
- **下一步断点**：在 GitHub 创建 `karmadesk` 仓库，并在本地终端执行推送命令，然后前往 Vercel 一键上线。

## 5. 最近完成

- [x] 完成 3D 对开推窗与深邃雨景全量调优；
- [x] 本地初始化 Git 仓库并完成生产提交；
- [x] 编写并归档 `docs/02_海外上线与部署运维SOP.md`；
- [x] 同步更新 `HANDOFF.md`。

## 6. 下一步上线执行清单

1. **GitHub 仓库创建与推送**：
   ```bash
   cd "/Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具"
   unset http_proxy https_proxy all_proxy HTTP_PROXY HTTPS_PROXY ALL_PROXY
   git remote add origin https://github.com/guoyixian2005/karmadesk.git
   git branch -M main
   git push -u origin main
   ```
2. **Vercel 一键导入上线**：
   - 登录 [vercel.com](https://vercel.com)，Import `karmadesk` 仓库，点击 Deploy 即刻上线生成全球公网链接。
3. **Gumroad 商品发布与替换**：
   - 在 Gumroad 上架 $4.99 典藏版商品，将商品真实链接填入 `index.html`。
4. **社媒冷启动**：
   - 基于 `docs/02_` 策略在 TikTok / Reddit / X 发布 10 秒桌面雨景微视频。

## 7. 关键文件索引

| 路径 | 说明 |
| :--- | :--- |
| [index.html](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/index.html) | 生产就绪型完整单页应用（直接双击浏览器秒开） |
| [docs/02_海外上线与部署运维SOP.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/02_海外上线与部署运维SOP.md) | GitHub 推送、Vercel 上线与 Gumroad 详细实操步骤 |
| [docs/01_产品需求文档_PRD.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/01_产品需求文档_PRD.md) | 完整 PRD 规范（功能、音效模型、定价与获客） |
| [docs/00_备选出海方向储备池.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/00_备选出海方向储备池.md) | 储备方向 A（社交凭证生成器）与 B（文字转卡片）备忘 |
| [HANDOFF.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/HANDOFF.md) | 项目唯一事实来源与执行断点 |
