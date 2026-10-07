# KarmaDesk (Project06) — 海外极速上线与部署运维 SOP

> **项目属性**：纯静态前端 Web 应用（零服务器成本、零数据库、全球 Anycast CDN）  
> **推荐生产平台**：Vercel Serverless / Cloudflare Pages（完全免费，自带全球 HTTPS 证书）

---

## 一、 第一步：创建 GitHub 仓库并推送代码

本项目已在本地完成 Git 初始化与首次全量提交。

### 1. 终端执行命令（在 Mac 终端中运行）
```bash
cd "/Users/guoyixian/Desktop/WB工作文件夹/Project06_数字疗愈解压工具"

# 1. 临时清除终端代理干扰（避免 Git 握手失败）
unset http_proxy https_proxy all_proxy HTTP_PROXY HTTPS_PROXY ALL_PROXY

# 2. 关联你的 GitHub 仓库（前往 github.com/new 创建一个名为 karmadesk 的公开/私有仓库）
git remote add origin https://github.com/guoyixian2005/karmadesk.git
git branch -M main

# 3. 推送至 GitHub
git push -u origin main
```

---

## 二、 第二步：Vercel 零配置秒级上线

1. **登录 Vercel**：访问 [vercel.com](https://vercel.com) 用你的 GitHub 账号一键登录；
2. **导入项目**：
   - 点击 **Add New... ➔ Project**；
   - 在 GitHub 仓库列表找到 `karmadesk`，点击 **Import**；
3. **部署配置（纯静态，无需任何修改）**：
   - Framework Preset：`Other`（自动识别纯静态 HTML）
   - Root Directory：`./`
   - Build and Output Settings：留空默认
   - 点击 **Deploy**！
4. **验证上线**：
   - 约 10~15 秒内完成全球 Edge CDN 部署；
   - Vercel 会自动分配一个极速的 `https://karmadesk-xxx.vercel.app` 免费生产域名。

---

## 三、 第三步：绑定自定义域名（可选，提升品牌信任度）

若想拥有专属独立域名（如 `karmadesk.app` 或二级域名 `zen.comilla.world`）：
1. 在 Vercel 项目后台进入 **Settings ➔ Domains**；
2. 输入你的域名（例如 `zen.comilla.world`）；
3. 根据 Vercel 提示，前往你的域名 DNS 控制台（Cloudflare / NameSilo）添加一条 `CNAME` 解析记录；
4. 几分钟内 Vercel 会自动免费签发 Let's Encrypt SSL 泛域名证书。

---

## 四、 第四步：Gumroad $4.99 收银台配置

1. **登录 Gumroad**：访问 [gumroad.com](https://gumroad.com)；
2. **新建商品**：
   - 点击 **Products ➔ New Product**；
   - Type 选 **Digital Product**；
   - Name 输入：`KarmaDesk Pro — Lifetime Zen Pass`；
   - Price 设置为：`$4.99`（一次性付费）；
3. **获取商品链接**：
   - 保存发布后，复制你的商品直链（例如 `https://xxx.gumroad.com/l/karmadesk`）；
4. **替换前端代码中的链接**：
   - 打开 `index.html`，搜索 `https://gumroad.com`，替换为你的真实商品直达链接；
   - 终端执行 `git commit -am "chore: update real gumroad product link" && git push`，Vercel 会自动秒级热更新生产环境。

---

## 五、 第五步：冷启动流量承接与转化

| 渠道 | 发帖策略与话术方向 | 推荐标签 |
| :--- | :--- | :--- |
| **TikTok / Reels** | 拍摄真实的电脑副屏挂着空山雨景，轻敲颂钵听清脆铜音，配文：“POV: You finally found the antidote to corporate burnout. Desk sanctuary for deep focus.” | `#WFH` `#cozydesk` `#desksetup` `#manifestation` `#asmr` |
| **Reddit** | 在 `r/CozyPlaces`, `r/InternetIsBeautiful`, `r/productivity` 发分享帖：“I built a zero-subscription minimalist desk sanctuary for my own burnout during WFH.” | 原创极简工具、免费试玩 |
| **Product Hunt** | 提交产品，突出“零订阅月费、无干扰、纯代码程序声疗”的独立创客故事。 | Productivity, Meditation |
