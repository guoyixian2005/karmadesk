# HANDOFF — Project06_数字疗愈解压工具 (KarmaDesk)

> 最后更新：2026-10-08 | 更新人：Gemini Spark (产品经理角色) | 交接给：人类 / 运维运营团队
> 规则：本文件是项目的「唯一事实来源」，**接手者必须先读本文件**。

## 1. 项目一句话概述

面向欧美年轻远程办公者与创作者的“3D对开推窗 · 灵签律动”微声疗与显化避难所（KarmaDesk v18.0 声学引擎极致重构与零卡顿暂停修复版），已完成全量产品调优与本地 Git 提交。

## 2. 技术栈 / 环境

- **前端技术栈**：HTML5 + Tailwind CSS + 原生 JavaScript + Web Audio API（136.1Hz 真实厚重铜钵声波 + 矿物敲击溪石 + 四音微风风铃 + 5 大高保真环境声景）+ 3D 对开推窗视差系统
- **声学引擎极致优化与卡顿/暂停 Bug 彻底修复 (Audio Engine & Pause Fix)**：
  1. **彻底解决暂停依然播放的 Bug**：重构为统一的 `stopAmbientSound()` 闭包回收器，点击暂停时瞬间切断全局节点指针、取消周期性音效定时器并阻断所有异步定时器冲突，彻底杜绝孤儿音频节点（Orphan Nodes）后台死循环播放；
  2. **消除音频循环缝隙爆音与卡顿**：重构了 `createSeamlessBuffer()`，使用 0.5 秒余弦等能量交叉淡入淡出（Cosine Crossfade），实现首尾振幅与导数 100% 平滑连续，无限循环播放零卡顿、零杂音、零爆音；
  3. **修复 Canvas 多重并发绘制泄漏**：严格生命周期管理（`startRainCanvas()` 与 `stopRainCanvas()`），每次暂停显式调用 `cancelAnimationFrame`，避免多次点击导致多个动画循环在后台叠加抢占 CPU/GPU；
  4. **5 大环境声景逼真度与解压质感全面升级**：
     - 🌧️ **Spring Mountain Rain**：双重低通温润粉噪 + 细密窗棂微滴雨韵；
     - ❄️ **Kyoto Snow Temple**：低回冬日微风呼啸 + 真实古铜寺庙大钟（92.5Hz 基频，每隔 22 秒深沉回荡，11 秒自然衰减）；
     - ⛈️ **Midnight Mountain Thunder**：窗外急雨 + 真实远山滚雷（38Hz–75Hz 次低频沉闷回响，每隔 19 秒群山轰鸣）；
     - 🎋 **Bamboo Brook Stream**：双共振带通滤波器模拟山涧清溪撞击竹筒与卵石的真实潺潺流水；
     - 🌊 **Deep Ocean Tide**：9 秒完整呼吸周期的深海潮汐涨落（4.5s 涌浪 + 4.5s 退沫），白噪音自适应扫频。
  5. **4 大案头圣物音效质感极致提升**：
     - 西藏铜磬：136.1Hz 地球 Om 频率 + 137.8Hz 物理拍频 + 408.3Hz/544.4Hz/816.6Hz 丰富高阶泛音，延音长达 9 秒，直击心灵；
     - 紫晶金字塔：升级为 C7–B7 高频空灵金字塔音疗鸣响，晶莹剔透；
     - 禅意溪石：高密度 1250Hz 矿物撞击瞬间 + 160Hz 深沉硬木案头回响，手感扎实沉稳；
     - 檐下风铃：日本江户风铃（Fururin）五音五度微风拂动，错落有致。
- **界面语言**：100% 地道纯正英文（零中文字符），海外直连。
- **交付形态**：纯静态单文件 Web 应用（直接双击 `index.html` 即可运行），零后端服务器维护成本，支持一键部署至 Vercel / Cloudflare Pages。
- **线上域名**：`https://karmadesk.comilla.world` / `https://karmadesk.vercel.app`。

## 3. 当前状态

阶段：**v18.0 声学引擎极致重构与零卡顿暂停修复版完成，本地已提交，推送到 GitHub 触发 Vercel 自动部署** (100%)。

## 4. 关键文件索引

| 路径 | 说明 |
| :--- | :--- |
| [index.html](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/index.html) | v18.0 声学引擎极致重构与零卡顿暂停修复版完整单页应用（直接双击浏览器秒开） |
| [docs/02_海外上线与部署运维SOP.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/02_海外上线与部署运维SOP.md) | GitHub 推送、Vercel 上线与 Gumroad 详细实操步骤 |
| [docs/01_产品需求文档_PRD.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/01_产品需求文档_PRD.md) | 完整 PRD 规范（功能、音效模型、定价与获客） |
| [docs/00_备选出海方向储备池.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/docs/00_备选出海方向储备池.md) | 储备方向 A（社交凭证生成器）与 B（文字转卡片）备忘 |
| [HANDOFF.md](file:///Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具/HANDOFF.md) | 项目唯一事实来源与执行断点 |
