# 外链建设详细指南

> 本文档记录每个外链网站的具体操作方法、入口、链接属性和示例。
> 持续更新中，目前已完成 10 个网站的研究。

---

## 1. GitHub (github.com)

**DA**: 100 | **费用**: 免费 | **类型**: 开发者平台

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Profile Bio/Blog | Settings → Public profile → Blog 字段 | Nofollow | 中 |
| 仓库 README | 创建公开仓库 → 添加 README.md → 写入链接 | Nofollow | 中 |
| **GitHub Pages** | **创建 `username.github.io` 仓库 → Settings → Pages** | **Dofollow** | **高** |
| 仓库 About/Website | 仓库主页 → About 齿轮 ⚙️ → Website 字段 | Nofollow | 低-中 |
| Profile README | 创建与用户名同名的仓库 → 添加 README.md | Nofollow | 中 |

### 操作步骤（推荐：GitHub Pages）

1. 创建仓库，命名为 `你的用户名.github.io`
2. 进入仓库 → Settings → Pages
3. Source 选择 `main` 分支
4. 在 `index.html` 中放置指向你网站的链接
5. 这是 GitHub 上**唯一的 dofollow 方法**

### 示例

- Linus Torvalds Profile: `https://github.com/torvalds` — Bio 下方显示网站链接
- 任意 `username.github.io` 站点中的 `<a href>` 链接默认 dofollow

### Tips

- 所有位置都填满（Bio、Blog URL、每个仓库的 Website）
- 创建有价值的 awesome-xxx 资源列表仓库，自然包含你的网站链接
- 保持活跃，定期 commit 的仓库更容易被抓取
- 不要批量创建空仓库只为放链接，会被标记 spam

---

## 2. Medium (medium.com)

**DA**: 95 | **费用**: 免费 | **类型**: 内容平台

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Profile Bio | Settings → Bio 字段 | **Dofollow** | 中 |
| **文章内链接** | **Write → 选中文字 → Ctrl+K → 粘贴 URL** | **Dofollow** | **高** |
| Publication 导航 | 创建 Publication → 设置导航链接 | **Dofollow** | 中 |
| 评论区链接 | 文章评论 | Nofollow | 低 |

### 操作步骤（推荐：文章内链接）

1. 注册 Medium 免费账户
2. 点击右上角 Write 按钮
3. 撰写 300+ 字的原创文章（与你网站主题相关）
4. 选中锚文本 → 点击链接图标（或 Ctrl+K）→ 粘贴目标 URL
5. 添加 Tags（最多 5 个）→ 发布

### 示例

- HubSpot: `https://medium.com/hubspot` — 文章大量链接回 hubspot.com
- Buffer: `https://medium.com/buffer-resources` — 文章链接回 buffer.com

### Tips

- Medium 文章内链接是 **dofollow**（`rel="noopener follow"`），极有价值
- 每篇文章只放 1-2 个外链，不要堆砌
- 写有独立价值的内容（80% 有用内容 + 20% 引导链接）
- 不要和主站发完全相同的内容（重复内容问题）
- 申请加入热门 Publication 增加曝光量
- Google 对 Medium 内容收录速度很快

---

## 3. Tumblr (tumblr.com)

**DA**: 90+ | **费用**: 免费 | **类型**: 博客/社交

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Profile Description | Settings → 博客设置 → Description | Nofollow | 低 |
| 博客文章正文 | Dashboard → New Post → 插入链接 | Nofollow | 中 |
| **自定义主题 HTML** | **Settings → Edit theme → Edit HTML → 手动写 `<a href>`** | **Dofollow** | **高** |
| **自定义页面 (Custom Layout)** | **Edit theme → Add a page → Custom Layout** | **Dofollow** | **中-高** |

### 操作步骤（推荐：自定义主题 HTML）

1. 注册 Tumblr，获得 `你的用户名.tumblr.com`
2. Settings → 你的博客 → Edit theme → Edit HTML
3. 在主题代码中（如 sidebar 或 footer）插入：
   ```html
   <a href="https://你的网站.com">你的锚文本</a>
   ```
4. 保存 — 这里的链接 Tumblr **不会自动添加 nofollow**
5. 另外发布几篇有内容的文章保持活跃

### 示例

- NASA Tumblr: `https://nasa.tumblr.com` — 描述和文章中链接回 nasa.gov
- 品牌站长：在自定义主题的 sidebar/footer 放 dofollow 链接

### Tips

- 自定义主题 HTML 是 Tumblr 上唯一可靠的 dofollow 方法
- 锚文本要多样化（品牌名、裸 URL、通用词混合）
- 每篇文章 300+ 字，图文并茂
- 利用 Reblog 机制扩散内容
- 一个博客只链一个网站，避免 link farm 嫌疑

---

## 4. Blogger / Blogspot (blogger.com)

**DA**: 高（Google 旗下） | **费用**: 免费 | **类型**: 博客平台

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 个人资料链接 | blogger.com/profile/edit → Homepage URL | Nofollow | 低 |
| 博客文章正文 | 新帖子 → 选中文字 → 链接图标 | Nofollow（默认） | 中 |
| HTML 编辑模式 | 文章编辑器 → 切换 HTML 视图 → 手写 `<a href>` | **可能 Dofollow** | 中-高 |
| 侧边栏小工具 | 布局 → 添加小工具 → HTML/JavaScript | **可能 Dofollow** | 低-中 |
| 博客模板 | 主题 → 编辑 HTML → 直接改模板源码 | **可能 Dofollow** | 中 |

### 操作步骤

1. 用 Google 账号登录 `blogger.com`
2. 创建博客 → 选地址（`xxx.blogspot.com`）
3. 发布 3-5 篇有实质内容的文章（300-500 字）
4. 文章中嵌入 1-2 个指向目标网站的链接
5. **关键**：切换到 HTML 编辑模式手写链接标签，有更大概率保持 dofollow

### 示例

Google 搜索 `site:blogspot.com "visit my website"` 可找到大量案例

### Tips

- Google 自家平台，收录速度快
- 一个 Google 账号不要创建太多博客（反垃圾检测）
- 给 Blogspot 博客本身也建几条外链（分层外链策略）
- 持续更新（每月 1-2 篇），避免被判定为废弃博客

---

## 5. WordPress.com (wordpress.com)

**DA**: 93-95 | **费用**: 免费 | **类型**: 博客平台

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 个人资料链接 | wordpress.com/me → Site URL 字段 | Nofollow | 低 |
| 博客文章链接 | wordpress.com/post → 正文插入链接 | Nofollow | 中 |
| 侧边栏 Widget | 外观 → 自定义 → Widgets → Custom HTML | Nofollow | 低 |
| 评论链接 | 他人博客评论 → Website 字段 | Nofollow | 低 |
| 页面链接 | wordpress.com/page → 新建页面 → 插入链接 | Nofollow | 中 |

### 操作步骤

1. 注册 `wordpress.com/start`（免费，无需信用卡）
2. 获得 `yourname.wordpress.com` 子域名
3. 点击 Write → 撰写文章 → 正文中插入链接
4. 发布

### Tips

- **所有链接均为 Nofollow**（WordPress.com 自 2005 年起全面 nofollow）
- 但 DA 93+ 的 nofollow 链接仍有品牌信号价值
- 文章要有价值（300+ 字），否则可能被判定 spam 删除
- 如果想要 dofollow，Medium 是更好的选择
- 作为外链组合的一环增加链接多样性

---

## 6. Behance (behance.net)

**DA**: 90+ | **费用**: 免费 | **类型**: 设计作品展示

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 个人资料 Website | 头像 → Edit Profile → Website 字段 | Nofollow | 中 |
| 项目描述链接 | Create a Project → 描述区选中文字 → 链接图标 | Nofollow | 中 |
| 项目信息栏 | 项目右侧 Project Info 面板 | Nofollow | 低 |

### 操作步骤

1. 注册 `behance.net`（可用 Adobe ID / Google）
2. 头像 → Edit Profile → Website 填入网站 URL
3. 创建项目 → 上传设计相关图片（至少 1 张）
4. 项目描述中自然插入网站链接
5. 添加 Tags 和 Creative Fields → 发布

### 示例

搜索 "website redesign" 可看到大量设计项目在描述中链接到客户网站

### Tips

- 所有链接 Nofollow，但 DA 90+ 有品牌曝光价值
- 上传高质量图片 — Google 图片搜索是额外流量来源
- 内容要与设计/创意相关，匹配平台定位
- 用品牌名注册（`behance.net/yourbrand`），有助品牌 SERP 占位

---

## 7. Issuu (issuu.com)

**DA**: 94 | **费用**: 免费（基础版） | **类型**: 文档发布平台

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 个人资料链接 | issuu.com/home/settings → Website 字段 | Nofollow | 中 |
| PDF 描述链接 | Upload PDF → Publication Settings → Description | Nofollow | 中 |
| PDF 内嵌链接 | 上传含超链接的 PDF → 阅读器保留链接 | Nofollow | 中 |

### 操作步骤

1. 注册 `issuu.com/signup`（免费）
2. Settings → Website 填入网站 URL
3. 上传一个 PDF（行业报告、教程、产品指南等）
4. 在 Publication Title 和 Description 中包含关键词和网站链接
5. 发布

### Tips

- PDF 标题含关键词，Issuu 页面本身会被 Google 索引
- Description 写 200-300 字描述，自然嵌入链接
- PDF 内容至少 5-10 页，过短价值低
- 可上传多个 PDF，每个针对不同关键词
- 用品牌名作为用户名（URL: `issuu.com/品牌名`）

---

## 8. About.me (about.me)

**DA**: 90+ | **费用**: 免费（基础版） | **类型**: 个人主页

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Website Link | Edit Page → Web Address 字段 | Nofollow | 中 |
| Social Links | Edit Page → Links 区域 → 添加社交链接 | Nofollow | 低 |
| CTA Button | Edit Page → CTA 按钮设置 | Nofollow | 中 |
| Bio 文本 | Edit Page → Bio（纯文本，不可加超链接） | — | 低 |

### 操作步骤

1. 注册 `about.me/signup`
2. 编辑页面 → Website 填入网站 URL
3. 添加所有社交链接
4. 写 Bio 包含品牌名和关键词
5. 上传高质量背景图

### 示例

- Tim Ferriss: `https://about.me/timferriss`
- 页面展示：大背景图 + 姓名 + Bio + Website 按钮 + 社交图标

### Tips

- 5 分钟设置完成，属于基础外链标配
- 用品牌名作为用户名（`about.me/yourbrand`）
- 配合 Gravatar、LinkedIn、GitHub 等形成品牌身份网络

---

## 9. Flickr (flickr.com)

**DA**: 90+ | **费用**: 免费（1000 张配额） | **类型**: 图片分享

### ⚠️ 链接属性更正

原文档标注 Flickr 为 **Dofollow**，经研究验证实际为 **Nofollow**。

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 个人资料 Website | Settings → Personal Information → Website | Nofollow | 中 |
| 照片描述 | 上传照片 → Description 中放 URL | Nofollow | 中 |
| 相册描述 | 创建相册 → 描述中放 URL | Nofollow | 低 |
| 群组讨论 | 加入群组 → Discussion 发帖放 URL | Nofollow | 低 |

### 操作步骤

1. 注册 `flickr.com`
2. Settings → Personal Information → Website 填入 URL
3. 上传 20-30 张高质量照片（与网站内容相关）
4. 照片描述中自然加入网站链接
5. 照片文件名用关键词（如 `best-seo-tools-2026.jpg`）

### Tips

- 照片本身会被 Google 图片搜索收录 — 间接流量
- 使用 Creative Commons 许可，让别人转载时保留署名链接
- Geo-tag 照片可用于本地 SEO
- 不要每张照片都放链接，会被标记垃圾

---

## 10. Gravatar (gravatar.com)

**DA**: 90+ | **费用**: 免费 | **类型**: 头像/个人资料服务

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Profile Links | gravatar.com/profile → Links → Add link | Nofollow | 中 |
| Verified Accounts | Profile → Verified Accounts → 关联社交平台 | Nofollow | 低 |
| Bio/About | Profile → About（纯文本） | — | 低 |

### 操作步骤

1. 注册 `gravatar.com`（与 WordPress.com 共享账号）
2. Profile → Links → Add link
3. Label 填关键词锚文本（如 "SEO工具"），URL 填网站地址
4. 可添加多个链接
5. 关联社交账号（Verified Accounts）

### 示例

- Matt Mullenweg: `https://gravatar.com/photomatt`

### Tips

- 5 分钟一次性设置，基础设施级别的外链
- Link 的 Label 用关键词作为锚文本优化
- 在 WordPress 博客评论时，头像自动链接到 Gravatar 资料页
- 多邮箱关联，扩大覆盖面
- 配合 WordPress 评论策略形成引流漏斗

---

## 汇总对比表

| 网站 | DA | 免费 | 最佳链接属性 | 操作难度 | 时间投入 | 推荐优先级 |
|------|-----|------|-------------|---------|---------|-----------|
| **GitHub Pages** | 100 | ✅ | **Dofollow** | 中 | 30min | ⭐⭐⭐⭐⭐ |
| **Medium 文章** | 95 | ✅ | **Dofollow** | 中 | 30min/篇 | ⭐⭐⭐⭐⭐ |
| **Tumblr 主题HTML** | 90+ | ✅ | **Dofollow** | 中 | 20min | ⭐⭐⭐⭐ |
| Blogger HTML模式 | 高 | ✅ | 可能 Dofollow | 低 | 15min | ⭐⭐⭐ |
| WordPress.com | 93 | ✅ | Nofollow | 低 | 15min | ⭐⭐⭐ |
| Behance | 90+ | ✅ | Nofollow | 低 | 15min | ⭐⭐⭐ |
| Issuu | 94 | ✅ | Nofollow | 低 | 10min | ⭐⭐⭐ |
| About.me | 90+ | ✅ | Nofollow | 极低 | 5min | ⭐⭐ |
| Flickr | 90+ | ✅ | Nofollow | 低 | 15min | ⭐⭐ |
| Gravatar | 90+ | ✅ | Nofollow | 极低 | 5min | ⭐⭐ |
