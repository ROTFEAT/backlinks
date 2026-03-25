# 外链建设详细指南

> 本文档记录每个外链网站的具体操作方法、入口、链接属性和示例。
> 持续更新中，目前已完成 150 个网站的研究。

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

---

# 二、Search Engine 搜索引擎类

> 通用方法：向搜索引擎提交网站索引，让搜索引擎收录你的网站。非传统外链，但对 SEO 基础极其重要。

## 11. Google (google.com)

**DA**: 100 | **费用**: 免费 | **类型**: 搜索引擎

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Google Search Console | search.google.com/search-console | 自然引用 | 极高 |
| Google Business Profile | business.google.com | Nofollow | 高（本地SEO） |

### 操作步骤

1. 访问 https://search.google.com/search-console
2. 添加网站资源（域名验证或 URL 前缀验证）
3. 提交 sitemap.xml
4. 使用"URL 检查"工具请求索引特定页面

### Tips

- Google Search Console 是所有 SEO 工作的基础，必须第一个设置
- Google Business Profile 对本地 SEO 极其重要，链接虽 nofollow 但直接影响本地搜索排名
- 提交 sitemap 后通常 24-48 小时内开始收录

## 12. Baidu 百度 (baidu.com)

**DA**: 100 | **费用**: 免费 | **类型**: 搜索引擎

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 百度搜索资源平台 | ziyuan.baidu.com | 自然引用 | 极高（中文市场） |

### 操作步骤

1. 访问 https://ziyuan.baidu.com
2. 注册百度账号并验证站点
3. 提交 sitemap 或使用主动推送 API
4. 也可手动提交 URL

### Tips

- 对中文网站必做
- 百度百科、百度知道等产品中的链接通常为 nofollow，且审核严格

## 13. Bing (bing.com)

**DA**: 100 | **费用**: 免费 | **类型**: 搜索引擎

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Bing Webmaster Tools | bing.com/webmasters | 自然引用 | 高 |
| Bing Places | bingplaces.com | Nofollow | 高（本地SEO） |

### 操作步骤

1. 访问 https://www.bing.com/webmasters
2. 可直接导入 Google Search Console 数据
3. 提交 sitemap
4. 支持 IndexNow 协议实现即时索引

### Tips

- 提交到 Bing 同时覆盖 Yahoo、AOL、DuckDuckGo
- IndexNow 协议一次提交多引擎受益

## 14. Yahoo (yahoo.com)

**DA**: 100 | **费用**: 免费 | **类型**: 搜索引擎

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 通过 Bing Webmaster Tools | bing.com/webmasters | 自然引用 | 中 |

### 操作步骤

1. Yahoo 搜索结果由 Bing 提供
2. 在 Bing Webmaster Tools 中提交即可自动覆盖 Yahoo
3. 无需单独提交

### Tips

- 无独立站长工具，Bing 提交即可

## 15. Yandex (yandex.com)

**DA**: 95+ | **费用**: 免费 | **类型**: 搜索引擎

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Yandex Webmaster | webmaster.yandex.com | 自然引用 | 高（俄语市场） |

### 操作步骤

1. 访问 https://webmaster.yandex.com
2. 注册 Yandex 账号并验证站点
3. 提交 sitemap
4. 支持 IndexNow 协议

### Tips

- 对俄语市场有重要价值
- 有独立爬虫和排名算法
- 界面支持英文

## 16-20. AOL / Ask.com / WolframAlpha / DuckDuckGo / Startpage

**费用**: 免费 | **类型**: 搜索引擎

这 5 个搜索引擎**无需单独提交**：
- **AOL** → 由 Bing 驱动，Bing 提交即覆盖
- **DuckDuckGo** → 主要来自 Bing 索引，Bing 提交即覆盖
- **Startpage** → Google 的隐私代理，Google 提交即覆盖
- **Ask.com** → 聚合多来源，无独立提交工具
- **WolframAlpha** → 计算知识引擎，不抓取网页，无法提交

### 实际只需操作 4 个平台

1. **Google Search Console** → 覆盖 Google + Startpage
2. **Bing Webmaster Tools** → 覆盖 Bing + Yahoo + AOL + DuckDuckGo
3. **Yandex Webmaster** → 覆盖 Yandex
4. **百度搜索资源平台** → 覆盖百度

---

# 三、Social 社交媒体类

> 通用方法：注册账号 → 个人资料/简介中添加网站链接。部分平台的帖子/文章内链接为 dofollow。

## 21. Facebook (facebook.com)

**DA**: 96 | **费用**: 免费 | **类型**: 社交媒体

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 个人资料"关于"页 | 个人资料 → 关于 → 联系方式和基本信息 → 网站 | Nofollow | 中 |
| 帖子中贴链接 | 发布帖子 → 粘贴 URL | Nofollow | 低 |
| 公共主页 | 创建公共主页 → 关于 → 网站 | Nofollow | 中 |

### 操作步骤

1. 登录 Facebook
2. 个人资料 → 关于 → 联系方式和基本信息
3. 在"网站"字段添加你的网站 URL
4. 保存

### Tips

- 所有外链均为 nofollow（`rel="nofollow noopener"`）
- 创建公共主页（Page）比个人账号更有 SEO 价值
- 帖子中的链接会生成预览卡片，增加点击率

## 22. Twitter/X (twitter.com)

**DA**: 94 | **费用**: 免费 | **类型**: 社交媒体

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Bio 网站字段 | 个人资料 → 编辑资料 → 网站 | Nofollow | 中 |
| 推文中链接 | 发推 → 粘贴 URL（通过 t.co 跳转） | Nofollow | 低 |

### 操作步骤

1. 登录 Twitter/X
2. 个人资料 → Edit profile
3. 在 Website 字段填入 URL
4. 保存

### Tips

- 所有链接通过 t.co 短链接跳转，均为 nofollow
- 推文被转发越多，间接 SEO 价值越大

## 23. LinkedIn (linkedin.com)

**DA**: 98 | **费用**: 免费 | **类型**: 职业社交

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **个人资料联系信息** | **资料 → 联系信息 → 网站** | **Dofollow** | **高** |
| 个人资料"精选"区域 | 资料 → 精选 → 添加链接 | Nofollow | 中 |
| 帖子/文章中链接 | 发布帖子或文章 → 插入链接 | Nofollow | 中 |

### 操作步骤

1. 登录 LinkedIn
2. 个人资料 → 联系信息 → 编辑
3. 在"网站"字段添加 URL（可选择标签：个人、公司、博客等）
4. 保存

### Tips

- 个人资料中的网站链接是 **dofollow**，LinkedIn 是少数给 dofollow 的大平台
- DA 98 极高，个人资料链接 SEO 价值很好
- 文章（Articles）内链接为 nofollow

## 24. Pinterest (pinterest.com)

**DA**: 94 | **费用**: 免费 | **类型**: 图片社交

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **Pin 目标 URL** | **创建 Pin → 添加目标链接** | **Dofollow** | **高** |
| 个人资料网站 | Settings → 认领网站 | Nofollow | 中 |

### 操作步骤

1. 注册 Pinterest 账号
2. 创建 Pin → 上传图片 → 添加目标 URL
3. Settings → 认领网站（增加可信度）
4. 每个 Pin 都可以附带一个目标链接

### Tips

- Pin 中的链接为 **dofollow**，Pinterest 是少数给 dofollow 的大平台之一
- 认领网站后效果更佳
- 高质量图片的 Pin 更容易被推荐和转发

## 25. Reddit (reddit.com)

**DA**: 97 | **费用**: 免费 | **类型**: 社区论坛

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 帖子/评论中链接 | 发帖或评论 → 插入链接 | Nofollow | 中（间接） |
| 个人资料 | 个人资料 → About 区域 | Nofollow | 低 |

### 操作步骤

1. 注册 Reddit 账号
2. 加入相关 subreddit
3. 发布有价值的内容，自然插入链接
4. 个人资料中也可添加网站链接

### Tips

- 所有链接 nofollow，但 Reddit 页面本身权重极高，被 Google 收录后间接有 SEO 价值
- 纯粹为了发链接会被版主删帖甚至封号
- 先养号积累 karma，再适当分享

## 26. Instagram (instagram.com)

**DA**: 93 | **费用**: 免费 | **类型**: 图片社交

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Bio 链接 | 个人资料 → 编辑资料 → 网站 | Nofollow | 低 |
| Stories 链接贴纸 | 发布 Story → 链接贴纸 | Nofollow | 低 |

### 操作步骤

1. 登录 Instagram
2. 个人资料 → 编辑资料
3. 在"网站"字段填入 URL
4. 保存

### Tips

- Bio 只能放 1 个链接（可用 Linktree 类工具扩展）
- 帖子正文中的链接**不可点击**
- 所有链接均为 nofollow

## 27. Vimeo (vimeo.com)

**DA**: 96 | **费用**: 免费（基础版） | **类型**: 视频平台

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **个人资料网站** | **Settings → Profile → Website** | **Dofollow** | **高** |
| 视频描述 | 上传视频 → 描述中放链接 | Dofollow | 中 |

### 操作步骤

1. 注册 https://vimeo.com/join
2. Settings → Profile
3. 在 Website 字段填入 URL
4. 上传视频，描述中也可放链接

### Tips

- Vimeo 个人资料链接为 **dofollow**，DA 96 极高
- 视频描述链接也被报告为 dofollow
- 高价值 dofollow 外链来源，优先级很高

## 28. Substack (substack.com)

**DA**: 90+ | **费用**: 免费 | **类型**: Newsletter 平台

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **文章正文链接** | **Write → 文章中插入链接** | **Dofollow** | **高** |
| 出版物首页 | Settings → 网站链接 | Dofollow | 中 |

### 操作步骤

1. 注册 https://substack.com
2. 创建出版物
3. 撰写文章，正文中插入目标网站链接
4. 发布

### Tips

- 文章正文中的链接为 **dofollow**，DA 高，SEO 价值很好
- 平台从付费订阅抽成 10%，但发布免费文章完全免费
- 高质量外链来源之一

## 29. Steemit (steemit.com)

**DA**: 70+ | **费用**: 免费 | **类型**: 区块链博客

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **文章正文链接** | **发布文章 → Markdown 链接** | **Dofollow** | **中-高** |
| 个人资料 | Settings → Website | Dofollow | 中 |

### 操作步骤

1. 注册 https://steemit.com（需要等待审批或通过第三方注册）
2. 撰写文章（支持 Markdown）
3. 在正文中用 `[锚文本](URL)` 插入链接
4. 发布

### Tips

- 文章正文链接为 **dofollow**，少数给 dofollow 的平台之一
- 注册可能需要等待几天审批
- 基于区块链，内容一旦发布无法删除

## 30-53. 其他社交平台速查

以下平台方法相同：注册 → 个人资料/简介 → 添加网站 URL。

| # | 网站 | 链接属性 | 费用 | 特殊说明 |
|---|------|----------|------|----------|
| 30 | TikTok | Nofollow | 免费 | 需 1000 粉丝或商业账号才能放链接 |
| 31 | Snapchat | Nofollow | 免费 | 公开 Profile 页可放链接 |
| 32 | Threads.net | Nofollow | 免费 | 链接继承 Instagram 设置 |
| 33 | Mastodon.social | **个人资料 Dofollow**（含 rel="me"） | 免费 | 支持多个链接验证，帖子链接 nofollow |
| 34 | Hive.blog | **文章 Dofollow** | 免费 | 与 Steemit 类似，文章链接 dofollow |
| 35 | Ghost.org | **文章 Dofollow** | 自托管免费/$9月起 | 默认 dofollow，SEO 价值很好 |
| 36 | Beehiiv.com | **文章 Dofollow** | 免费（基础版） | Newsletter 文章链接 dofollow |
| 37 | Dailymotion | Nofollow | 免费 | 视频描述和个人资料可放链接 |
| 38 | Twitch.tv | Nofollow | 免费 | 频道面板可放链接 |
| 39 | Telegram.org | Nofollow | 免费 | 内容不被搜索引擎索引，无 SEO 价值 |
| 40 | Discord.com | Nofollow | 免费 | 内容不被搜索引擎索引，无 SEO 价值 |
| 41 | Rumble.com | Nofollow | 免费 | 视频描述和频道信息可放链接 |
| 42 | VK.com | Nofollow | 免费 | 俄语社交平台，个人资料可放链接 |
| 43 | Truth Social | Nofollow | 免费 | 个人资料可放链接 |
| 44 | Gab.com | Nofollow | 免费 | Bio 和帖子可放链接 |
| 45 | Gettr.com | Nofollow | 免费 | Bio 可放链接 |
| 46 | Parler.com | Nofollow | 免费 | 平台状态不稳定 |
| 47 | Odysee.com | Nofollow | 免费 | 视频/频道描述可放链接 |
| 48 | Spotify (Podcasters) | Nofollow | 免费 | Show Notes 可放链接 |
| 49 | Locals.com | Nofollow | 免费 | 创作者页面"关于"可放链接 |
| 50 | ConvertKit/Kit.com | Nofollow | 免费（基础版） | Creator Profile 公开页可放链接 |
| 51 | Mixcloud.com | Nofollow | 免费 | 音频平台，个人资料可放链接 |
| 52 | Anchor.fm | Nofollow | 免费 | 已并入 Spotify for Podcasters |
| 53 | Bitchute.com | Nofollow | 免费 | 视频描述可放链接 |

### 社交平台 Dofollow 优先级

1. **LinkedIn 个人资料** (DA 98) — 必做
2. **Pinterest Pin 链接** (DA 94) — 每个 Pin 都是 dofollow
3. **Vimeo 个人资料** (DA 96) — 必做
4. **Substack 文章** (DA 90+) — 写文章获得 dofollow
5. **Ghost 文章** — 自托管完全控制
6. **Steemit/Hive.blog 文章** — 文章链接 dofollow
7. **Beehiiv 文章** — Newsletter 链接 dofollow
8. **Mastodon 个人资料** — 支持 rel="me" 验证


---

# 四、Review Sites 点评类

> 通用方法：注册商家/产品页面 → 填写公司信息和网站 URL → 验证商家身份。大部分需要商家验证（电话/邮件/邮寄）。

## 54. Yelp (yelp.com)

**DA**: 93 | **费用**: 免费 | **类型**: 本地商家点评

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 商家资料网站链接 | Yelp for Business → 添加商家 → 网站URL | Nofollow | 高（本地SEO） |

### 操作步骤

1. 访问 https://biz.yelp.com
2. 认领或添加商家信息
3. 填写网站 URL
4. 通过电话/邮件/邮寄验证商家

### Tips

- 虽 nofollow 但对本地 SEO 排名和品牌信任度极重要
- 需要真实商家信息验证

## 55. TripAdvisor (tripadvisor.com)

**DA**: 93 | **费用**: 免费 | **类型**: 旅游点评

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 商家资料网站链接 | TripAdvisor for Business → 认领商家 → 网站URL | Nofollow | 高（旅游SEO） |

### 操作步骤

1. 访问 https://www.tripadvisor.com/Owners
2. 认领或添加商家
3. 填写网站链接
4. 验证（仅限旅游/餐饮/住宿类商家）

### Tips

- 仅限旅游、餐饮、住宿类商家
- 对旅游行业 SEO 极重要

## 56. Trustpilot (trustpilot.com)

**DA**: 93 | **费用**: 免费（基础版） | **类型**: 商家信誉评价

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 公司页面网站链接 | business.trustpilot.com → 创建公司页面 → 网站URL | Nofollow | 高 |

### 操作步骤

1. 访问 https://business.trustpilot.com
2. 注册并创建公司页面
3. 填写公司网站 URL
4. 通过 DNS 或邮件验证域名

### Tips

- 任何在线业务均可注册
- Trustpilot 页面在 Google 搜索中排名很好，有品牌 SERP 占位价值

## 57. G2 (g2.com)

**DA**: 92 | **费用**: 免费（基础版） | **类型**: 软件评价

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 产品页面链接 | seller.g2.com → 添加产品 → 官网URL | Nofollow | 高（SaaS） |

### 操作步骤

1. 访问 https://seller.g2.com
2. 添加/认领软件产品页面
3. 填写产品官网 URL
4. 需审核（仅限软件/SaaS 产品）

### Tips

- 仅限软件/SaaS 产品
- G2 页面 Google 排名很好，品牌 SERP 价值高

## 58-95. 其他点评平台

### 免费 + Dofollow 平台（优先操作）

| # | 网站 | 入口方法 | 链接属性 | 备注 |
|---|------|----------|----------|------|
| 58 | **brownbook.net** | Add a Business → 填商家信息含网站URL | **Dofollow** | 无需验证，极低门槛 |
| 59 | **hotfrog.com** | Add your business → 填商家信息含网站URL | **Dofollow** | 门槛低，适合快速获取 |
| 60 | **manta.com** | Add your business → 填公司信息含网站URL | **Dofollow** | DA 较高，值得做 |
| 61 | **chamberofcommerce.com** | Add your business → 填商家信息含网站URL | **Dofollow** | DA 较高，需邮箱验证 |
| 62 | **tupalo.com** | 注册 → Add a place → 填商家信息含网站URL | **Dofollow** | 无需验证 |
| 63 | **cylex.com** | Add company → 填公司信息含网站URL | **Dofollow** | 基础免费 |
| 64 | **n49.com** | Add a Business → 填商家信息含网站URL | **Dofollow** | 主要面向加拿大市场 |
| 65 | **fyple.com** | Add business → 填商家信息含网站URL | **Dofollow** | 无需验证 |
| 66 | **tuugo.us** | Register your company → 填公司信息含网站URL | **Dofollow** | 基础免费 |
| 67 | **showmelocal.com** | Add your business → 填商家信息含网站URL | **Dofollow** | 基础免费 |

### 免费 + Nofollow 但核心必做平台

| # | 网站 | 入口方法 | 备注 |
|---|------|----------|------|
| 68 | **Google Business Profile** | business.google.com → 创建/认领商家 | 本地SEO核心，需验证 |
| 69 | **Bing Places** | bingplaces.com → 注册/认领商家 | 对Bing排名有直接帮助 |
| 70 | **Apple Maps Connect** | mapsconnect.apple.com → 添加/认领商家 | 提升品牌曝光 |
| 71 | **Foursquare** | business.foursquare.com → 认领商家 | 需电话/邮件验证 |

### 付费点评平台

| # | 网站 | 费用 | 链接属性 | 备注 |
|---|------|------|----------|------|
| 72 | **BBB.org** | 年费 $500+ | **Dofollow** | DA 93 极高权重，认证后价值很高 |
| 73 | **ConsumerAffairs** | 付费订阅 | Nofollow | 品牌管理功能需付费 |

### 软件/SaaS 专用平台

| # | 网站 | 入口 | 链接属性 |
|---|------|------|----------|
| 74 | Capterra | vendors.capterra.com → 提交产品 | Nofollow |
| 75 | GetApp | vendor portal → 提交产品 | Nofollow |
| 76 | Glassdoor | glassdoor.com/employers → 认领公司 | Nofollow |
| 77 | Indeed | indeed.com/hire → 创建公司页面 | Nofollow |
| 78 | Angi.com | business.angi.com → 添加服务商 | Nofollow |
| 79 | SiteJabber | sitejabber.com/businesses → 认领 | Nofollow |

### SaaS 管理工具（非目录站，不提供直接外链）

| # | 网站 | 说明 |
|---|------|------|
| 80-85 | Yext / BrightLocal / Vendasta / Podium / Birdeye / Reputation.com | 付费SaaS工具，帮你管理其他平台的listing，自身不提供外链 |
| 86-95 | YellowPages / SuperPages / DexKnows / Local.com / CitySearch / MapQuest / Spoke / JudysBook / Grade.us / NiceJob | 黄页/目录聚合站，大部分 Nofollow，通过各站 Claim listing 入口认领 |

---

# 五、URL Shortener 短链接类

> 通用方法：创建短链接，访问时通过 301 重定向跳转到目标 URL。大部分使用 301 重定向传递权重。

### 关键说明

URL 缩短服务的 SEO 价值**非常有限**。Google 明确表示能识别短链接并追踪到目标 URL，短链接本身几乎没有 PageRank。这些服务更适合用于链接追踪和社交分享，不应作为核心外链策略。

### 301 重定向类（传递权重，46 个）

| # | 网站 | 方法 | 免费 | 特殊说明 |
|---|------|------|------|----------|
| 96 | tinyurl.com | 创建短链接 → 301 跳转 | 免费 | 有付费增值 |
| 97 | bitly.com | 创建短链接 → 301 跳转 | 免费 | 有付费增值，支持品牌域名 |
| 98 | cutt.ly | 创建短链接 → 301 跳转 | 免费 | 有付费增值 |
| 99 | tiny.cc | 创建短链接 → 301 跳转 | 免费 | 有付费增值 |
| 100 | is.gd / v.gd | 创建短链接 → 301 跳转 | 免费 | 支持 +后缀查看预览 |
| 101 | rebrandly.com | 创建品牌短链接 → 301 跳转 | 免费 | 支持自定义域名 |
| 102 | kutt.it | 开源自托管短链接 → 301 跳转 | 免费开源 | 可自己部署 |
| 103-148 | bit.do / shorturl.at / rb.gy / gg.gg / u.to / tiny.pl / n9.cl / cutt.us / tr.im / urlzs.com / soo.gd / pnut.co / ity.im / qr.net / ai6.net / shrunken.com / al.ly / lnnkin.com / teil.cc / linksplit.io / cado.pro / bch.gg / vzturl.com / gcc.gl / qrurl.cc / corvoapp.com / mityurl.com / haggybear.com / vivoldi.com / shtn.me / ux.nu / chilp.it / picsee.co / shorl.com / zzb.bz / 0rz.tw / bom.to / linklyhq.com | 创建短链接 → 301 跳转 | 全部免费 | 标准短链接服务 |

### 不传递权重类（应避免）

| # | 网站 | 原因 |
|---|------|------|
| 149 | s.id | 302 重定向，不传递权重（但 Bio 页面有 dofollow 链接） |
| 150 | fc.lc | 明确 Nofollow + 302 重定向 |
| 151 | bc.vc / za.gl / shrtfly.com | 广告中间页型，Nofollow，用户体验差 |
| 152 | yellkey.com | 临时链接会过期，过期后外链失效 |

---

# 六、Deals 优惠类

> 通用方法：在优惠/团购平台发布产品折扣信息，商品页面或商家资料中包含网站链接。

### Dofollow 平台（优先操作）

## 153. RedFlagDeals Forums (forums.redflagdeals.com)

**DA**: 70+ | **费用**: 免费 | **类型**: 优惠论坛

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **论坛发帖** | **Hot Deals 版块 → 发帖分享优惠** | **Dofollow** | **中-高** |

### 操作步骤

1. 注册 https://forums.redflagdeals.com
2. 在 Hot Deals 版块点击发帖
3. 分享优惠信息，帖中带上网站链接
4. 即时发布

### Tips

- 本类中唯一的 Dofollow 来源
- 加拿大最大优惠论坛，流量大

## 154. UKAds (ukads.org)

**DA**: 中 | **费用**: 免费 | **类型**: 英国分类广告

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **发布广告** | **注册 → 发布优惠信息含链接** | **Dofollow** | **中** |

### 操作步骤

1. 注册 https://ukads.org
2. 选择分类发布广告
3. 描述中加入网站链接
4. 即时发布

### 其他 Deals 平台（Nofollow）

| # | 网站 | 入口 | 免费 | 备注 |
|---|------|------|------|------|
| 155 | SlickDeals | 注册 → Post a Deal → 填链接 | 免费 | 流量最大的优惠站 |
| 156 | Groupon | Merchant Center → 创建团购活动 | 按成交抽佣 | 需商家审核 |
| 157 | AppSumo | Partner Portal → Submit Product | 平台抽成 | 仅限 SaaS |
| 158 | DealSpotr | 注册 → Suggest a New Store → 发布优惠 | 免费 | |
| 159-176 | StackSocial / DealNews / Hip2Save / BradsDeals / MightyDeals / DontPayFull / DealFuel / PitchGround / BensBargains / Dealify / DealMirror / SaaSMantra / eDealInfo / GetsCoupon / DealsSourceForge / DealIgg / BootstrapPS / GetStartedHQ | 注册后提交优惠/产品信息 | 免费或抽佣 | 大部分 Nofollow |

---

# 七、Coupon 优惠券类

> 通用方法：注册后提交商家优惠券/折扣码，优惠详情页包含商家网站链接。几乎全部免费，几乎全部 Nofollow。

### Dofollow 平台

仅 **forums.redflagdeals.com**（与 Deals 类共享）的 Coupons 版块为 Dofollow。

### 推荐平台

| # | 网站 | 入口 | 免费 | 备注 |
|---|------|------|------|------|
| 177 | RetailMeNot | 通过 Affiliate 渠道或用户提交优惠码 | 免费/联盟佣金 | 最大优惠券站之一 |
| 178 | CouponChief | /coupons/submit → 提交优惠码 | 免费 | Pays-2-Share 可赚 2% 佣金 |
| 179 | CouponBirds | /submit-coupon → 提交优惠码+截图 | 免费 | 1-2 工作日审核 |
| 180-205 | SlickDeals / DealSpotr / DealNews / Hip2Save / DontPayFull / Meliuz / CouponClans / CouponSlasher / PromoCodes / EmuCoupon / BensBargains / MyCoupons / eDealInfo / GetsCoupon / ValidCoupons / EuaCupones / CouponX / Voucher.Ninja / DealCatcher / SharedCoupon / CouponScored / CouponSuper / Rebajas.Guru / CouponsSalmon / UCSB HR Discounts | 注册后提交优惠码/折扣信息 | 全部免费 | 全部 Nofollow |

---

# 八、Press Release 新闻稿类

> 通用方法：撰写新闻稿，稿件正文中嵌入公司网站链接，通过发稿平台分发。大部分收费。

### Dofollow 平台

## 206. ReleaseWire (releasewire.com)

**DA**: 中 | **费用**: 付费 | **类型**: 新闻稿发布

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **新闻稿内链接** | **注册 → 提交新闻稿 → 正文嵌入链接** | **Dofollow** | **中-高** |

### 操作步骤

1. 注册 https://releasewire.com
2. 撰写新闻稿
3. 正文中嵌入公司网站链接
4. 提交，即时发布

### Tips

- 本类中唯一确认的 Dofollow 链接来源
- 付费服务

### 免费新闻稿平台

| # | 网站 | 入口 | 免费额度 | 链接属性 |
|---|------|------|----------|----------|
| 207 | **OpenPR** (openpr.com/openpr.de) | /news/submit.html → 提交新闻稿 | 1篇/30天免费 | Nofollow |
| 208 | **PRSync** (prsync.com) | 注册 → 提交新闻稿 | 无限量免费 | Nofollow |
| 209 | **PR.com** | 注册 → 提交新闻稿 | 基础版免费 | Nofollow |
| 210 | **1888PressRelease** | 注册 → 提交新闻稿 | 免费/$15起增强 | Nofollow |
| 211 | **Express-Press-Release.net** | 注册 → 提交新闻稿 | 免费 | Nofollow |
| 212 | **OnlinePRNews** | 注册 → 提交新闻稿 | 基础版免费 | Nofollow |
| 213 | **MyPR.bg** | 注册 → 提交新闻稿（保加利亚） | 基础免费 | Nofollow |

### 付费新闻稿平台

| # | 网站 | 费用 | 备注 |
|---|------|------|------|
| 214 | PRWeb | $110-$455/篇 | 主流发稿平台 |
| 215 | Newswire | 按套餐 | |
| 216 | EINPresswire | $149/篇起 | 需2天验证 |
| 217 | Prowly | $258/月起 | PR 软件 |
| 218-227 | 24-7PressRelease / SBWire / Pressat / Vuelio / Dino.com.br / Pressemeddelelse.dk / RoxhillMedia / PRFire / PressHunt / MyPR.bg Pro | $15-$6000+/年 | 按各平台定价 |

---

# 九、Communities 社区类

> 通用方法：注册社区账号 → 发帖/评论/创建内容 → 个人资料或内容中放链接。

### Dofollow 社区（优先操作）

## 228. Fark (fark.com)

**DA**: 70+ | **费用**: 免费 | **类型**: 新闻聚合

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **提交新闻链接** | **注册 → 提交链接 → 编辑审核** | **Dofollow** | **中-高** |

### 操作步骤

1. 注册 https://fark.com
2. 提交新闻链接
3. 编辑筛选后上首页
4. 通过审核的链接为 dofollow

### Tips

- 需要编辑审核，非即时发布
- 提交有趣/新闻价值的内容更容易通过

## 229. BlackPlanet (blackplanet.com)

**DA**: 60+ | **费用**: 免费 | **类型**: 社交网络

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **个人资料链接** | **注册 → 个人资料 → 网站字段** | **Dofollow** | **中** |

### 操作步骤

1. 注册 https://blackplanet.com
2. 编辑个人档案
3. 在网站字段填入 URL
4. 保存

## 230. HerCampus (hercampus.com)

**DA**: 70+ | **费用**: 免费 | **类型**: 校园媒体

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| **文章内链接** | **申请 Campus Contributor → 撰写文章 → 嵌入链接** | **Dofollow** | **中-高** |

### 操作步骤

1. 访问 https://hercampus.com
2. 申请成为 Campus Contributor
3. 撰写文章，文内嵌入链接
4. 提交审核发布

### 其他 Dofollow 社区

| # | 网站 | 入口 | 链接属性 | 备注 |
|---|------|------|----------|------|
| 231 | us.community.sony.com | 注册 → 发帖/个人资料 | **Dofollow** | Sony 官方社区 |
| 232 | forum.unilang.org | 注册 → 发帖讨论语言学习 | **Dofollow** | 语言学习论坛 |
| 233 | 3dprintboard.com | 注册 → 发帖讨论 3D 打印 | **Dofollow** | vBulletin 论坛 |
| 234 | maxforlive.com | 注册 → 分享 Max for Live 设备 | **Dofollow** | 音乐制作社区 |
| 235 | worldswithoutend.com | 注册 → 写书评/论坛讨论 | **Dofollow** | 科幻书评社区 |
| 236 | fotografie.at | 注册 → 上传照片/个人资料 | **Dofollow** | 奥地利摄影社区 |
| 237 | painterfactory.com | 注册 → 参与讨论 | **Dofollow** | 数字绘画社区 |
| 238 | artforum.online | 注册 → 发帖讨论艺术 | **Dofollow** | 艺术论坛 |

### Nofollow 但高价值社区

| # | 网站 | 入口 | 备注 |
|---|------|------|------|
| 239 | StackOverflow | 注册 → 回答问题 → 个人资料放链接 | 声望<10限制链接数 |
| 240 | Quora | 注册 → 回答问题 → Bio/回答中放链接 | |
| 241 | Hacker News | 注册 → Show HN 发帖 → About 字段放链接 | 先养号 |
| 242 | SlashDot | 注册 → 评论/日志放链接 | |
| 243 | Dribbble | 注册 → 上传作品 → 个人资料放链接 | Pro $5/月 |
| 244 | IndieHackers | 注册 → 发帖/个人资料 | 2000 积分后 Dofollow |
| 245 | CodeProject | 注册 → 发文章 → Silver 会员可加签名超链接 | |
| 246 | MetaFilter | 注册（一次性 $5） → 发帖 | 严禁自我推广 |
| 247-276 | Meetup / PrestaShop / StackExchange / SuperUser / ServerFault / F6s / GrowthHackers / SelfGrowth / Meneame / UpLabs / TranslatorsCafe / HowLongToBeat / FimFiction / WebDesignerNews / AnimeForums / NYGunForum / BoredPanda / Steinberg / FotoCommunity / AuthorStream 等 | 注册 → 个人资料/帖子放链接 | 各站规则不同 |

### 已死亡/不可用（跳过）

- **ruqqus.com** — 2021 年已关闭
- **designernews.co** — 2024 年已死亡
- **pixelation.org** — 已归档，无法注册

---

# 十、Infographic 信息图类

> 通用方法：上传信息图 → 描述/来源中放入网站链接。

| # | 网站 | 入口 | 免费 | 链接属性 |
|---|------|------|------|----------|
| 277 | **SlideShare** | slideshare.net → 上传信息图(PPT/PDF) → 描述放链接 | 免费 | **Dofollow** |
| 278 | Visual.ly | visual.ly → 注册创作者 → 提交信息图 | 免费 | Nofollow |
| 279-285 | DailyInfographic / CoolInfographics / InfographicJournal / InfographicsArchive / InfographicBee / Gifographics / InfographicReviews | 通过 Submit 页面提交信息图 | 免费 | 待验证 |

---

# 十一、Article Submission 文章投稿类

> 通用方法：注册作者账号 → 发布/投稿文章 → 文章正文或 Author Bio 中嵌入链接。本类 Dofollow 比例最高（75%）。

### Dofollow 文章投稿站（15个）

| # | 网站 | 入口 | 链接属性 |
|---|------|------|----------|
| 286 | **Vingle** (vingle.net) | 注册 → 兴趣频道发文章 → 嵌入链接 | **Dofollow** |
| 287 | **Storeboard** (storeboard.com) | 注册商户 → Blog板块发文章 → 嵌入链接 | **Dofollow** |
| 288 | **Launchora** (launchora.com) | 注册 → 直接发文章 → 插入链接 | **Dofollow** |
| 289 | **ArticleTed** (articleted.com) | 注册 → 提交文章 → Author Bio/正文加链接 | **Dofollow** |
| 290 | **Articles.Gappoo** (articles.gappoo.com) | 注册 → 提交文章 → 正文嵌入链接 | **Dofollow** |
| 291 | **Articles.Studio9xb** (articles.studio9xb.com) | 注册 → 提交文章 → Bio 加链接 | **Dofollow** |
| 292 | **Articles.KraftLoft** (articles.kraftloft.com) | 注册 → 提交文章 → 正文/Bio 嵌入链接 | **Dofollow** |
| 293 | **PR4-Articles** (pr4-articles.com) | 注册 → 发布文章 → 正文加链接 | **Dofollow** |
| 294 | **PR5-Articles** (pr5-articles.com) | 注册 → 发布文章 → 正文加链接 | **Dofollow** |
| 295 | **PR3-Articles** (pr3-articles.com) | 注册 → 发布文章 → 正文加链接 | **Dofollow** |
| 296 | **PR7-Articles** (pr7-articles.com) | 注册 → 发布文章 → 正文加链接 | **Dofollow** |
| 297 | **Articles.SEOForums** (articles.seoforums.me.uk) | 注册 → 提交SEO相关文章 → 嵌入链接 | **Dofollow** |
| 298 | **Articles.JainKathaLok** (articles.jainkathalok.com) | 注册 → 提交文章 → 正文/Bio 加链接 | **Dofollow** |
| 299 | **Articles.MyBikaner** (articles.mybikaner.com) | 注册 → 提交文章 → 正文/Bio 加链接 | **Dofollow** |

### Nofollow 文章投稿站（5个）

| # | 网站 | 入口 |
|---|------|------|
| 300 | SooperArticles | 注册 → 提交文章 |
| 301 | Telescope.ac | 注册 → 创建频道发文章 |
| 302 | Blog.Shopolop | 注册 → 投稿博客文章 |
| 303 | Article.AdvertiseEra | 注册 → 提交文章 |
| 304 | BloggersRoad | 注册 → 提交 Guest Post |
| 305 | Tripod/Lycos | 创建免费网页/博客 → 页面内放链接 |

---

# 十二、File Upload 文件上传类

> 通用方法：上传文件（PDF/PPT/文档/图片/视频） → 描述或文件内容中包含链接。Dofollow 比例 62.5%。

### Dofollow 文件上传站（25个）

| # | 网站 | 入口方法 | 备注 |
|---|------|----------|------|
| 306 | **SlideShare** (slideshare.net) | 上传 PPT/PDF → 描述放链接 | 高权重 |
| 307 | **Calameo** (calameo.com) | 上传 PDF → 在线翻页杂志 → 描述放链接 | 高权重 |
| 308 | **FlipSnack** (flipsnack.com) | 上传 PDF → 转翻页电子书 → 描述放链接 | 基础版免费 |
| 309 | **Padlet** (padlet.com) | 创建公开看板 → 卡片中添加链接 | 免费限量 |
| 310 | **Wakelet** (wakelet.com) | 创建内容集合 → 添加链接卡片 | 免费 |
| 311 | **Hightail** (hightail.com) | 上传文件 → 分享空间描述放链接 | 基础版免费 |
| 312 | **GoNitro** (gonitro.com) | 上传 PDF → 描述放链接 | 基础版免费 |
| 313 | **Easel.ly** (easel.ly) | 创建信息图 → 描述放链接 | 免费 |
| 314 | **Files.fm** (files.fm) | 上传文件 → 描述放链接 | 免费 |
| 315 | **Emaze** (emaze.com) | 创建在线演示 → 内容嵌入链接 | 基础版免费 |
| 316 | **Edocr** (edocr.com) | 上传文档/PDF → 描述放链接 | 免费，高价值 |
| 317 | **Anotepad** (anotepad.com) | 创建公开笔记 → 内容放链接 | 免费，无需注册 |
| 318 | **Noti.st** (noti.st) | 上传演讲幻灯片 → 描述放链接 | 免费 |
| 319 | **ImageEvent** (imageevent.com) | 上传图片 → 相册描述放链接 | 免费 |
| 320 | **Docracy** (docracy.com) | 上传法律文档 → 描述放链接 | 免费 |
| 321 | **Chomikuj.pl** (chomikuj.pl) | 上传文件 → 描述放链接 | 免费（波兰站） |
| 322 | **Bit.ai** (bit.ai) | 创建文档并公开分享 → 嵌入链接 | 免费限量 |
| 323 | **CloudMe** (cloudme.com) | 上传文件 → 描述放链接 | 基础版免费 |
| 324 | **PDFSlide** (pdfslide.us) | 上传 PDF/PPT → 描述放链接 | 免费 |
| 325 | **SlideHTML5** (slidehtml5.com) | 上传 PPT/PDF → HTML5 幻灯片 → 描述放链接 | 免费 |
| 326 | **Clipix** (clipix.com) | 创建剪贴板 → 添加链接卡片 | 免费 |
| 327 | **SmugMug** (smugmug.com) | 上传图片 → 描述放链接 | 付费（有试用） |
| 328-331 | **Diode.zone / PeerTube.ch / P2PTV.ru / PeerVideo.ru** | 上传视频 → 描述放链接 | 免费（PeerTube 实例） |

### Nofollow 文件上传站（14个）

| # | 网站 | 入口 |
|---|------|------|
| 332 | ReadTheDocs | 托管文档项目 → 文档内放链接 |
| 333 | SpeakerDeck | 上传 PPT/PDF → 描述放链接 |
| 334 | 4Shared | 上传文件 → 描述放链接 |
| 335 | DocDroid | 上传文档 → 描述放链接 |
| 336 | Gifyu | 上传图片 → 描述放链接 |
| 337 | ItemFix | 上传视频 → 描述放链接 |
| 338 | iPernity | 上传图片 → 描述放链接 |
| 339 | PicturePush | 上传图片 → 描述放链接 |
| 340 | Mobissue | 上传 PDF → 移动电子书 → 描述放链接 |
| 341 | NetBoard.me | 创建内容面板 → 添加链接 |
| 342 | PhotoPeach | 上传图片 → 幻灯片描述放链接 |
| 343 | PowerShow | 上传 PPT → 描述放链接 |
| 344 | EasyZoom | 上传高分辨率图片 → 描述放链接 |
| 345 | Flaticon | 注册设计师 → 上传图标 → 个人页放链接 |

---

# 十三、Classified Ads 分类广告类

> 通用方法：注册后发布分类广告 → 广告描述中填入网站链接。大部分免费即时发布。Dofollow 比例 72%。

### Dofollow 分类广告站（39个）

| # | 网站 | 入口 | 地区 |
|---|------|------|------|
| 346 | **JustLanded** (justlanded.com) | 注册 → 海外生活分类发布广告 | 全球 |
| 347 | **AdlandPro** (adlandpro.com) | 注册 → 商业/服务分类发布广告 | 全球 |
| 348 | **FreeGlobalClassifiedAds** | 注册 → 全球分类发布广告 | 全球 |
| 349 | **Hot-Web-Ads** | 注册 → 分类发布广告 | 全球 |
| 350 | **CanetAds** | 注册 → 分类发布广告 | 全球 |
| 351 | **USAOnlineClassifieds** | 注册 → 美国地区分类发布广告 | 美国 |
| 352 | **iHubbub** | 注册 → 分类发布广告 | 全球 |
| 353 | **UKAdsList** | 注册 → 英国分类发布广告 | 英国 |
| 354 | **AunetAds** | 注册 → 澳大利亚分类发布广告 | 澳大利亚 |
| 355 | **InnetAds** | 注册 → 印度分类发布广告 | 印度 |
| 356 | **WallClassifieds** | 注册 → 分类墙发布广告 | 全球 |
| 357 | **GlobalClassified.net** | 注册 → 全球分类发布广告 | 全球 |
| 358 | **Classified4Free** | 注册 → 免费分类发布广告 | 全球 |
| 359 | **GBIBP** | 注册 → 商业分类发布广告 | 全球 |
| 360 | **FreeWebAds.biz** | 注册 → 分类发布广告 | 全球 |
| 361 | **FreeAdsOnline.biz** | 注册 → 分类发布广告 | 全球 |
| 362 | **PostHereAds** | 注册 → 发布广告 | 全球 |
| 363 | **Classifieds4Free.biz** | 注册 → 分类发布广告 | 全球 |
| 364 | **NextFreeAds** | 注册 → 分类发布广告 | 全球 |
| 365 | **FreeBestAds** | 注册 → 发布广告 | 全球 |
| 366 | **PostZoo** | 注册 → 分类目录发布广告 | 全球 |
| 367 | **GreatClassified** | 注册 → 分类发布广告 | 全球 |
| 368 | **LetsPostFree** | 注册 → 免费发布广告 | 全球 |
| 369 | **BabaAds** | 注册 → 分类发布广告 | 全球 |
| 370 | **GlobiAd** | 注册 → 全球分类发布广告 | 全球 |
| 371 | **CityAd.in** | 注册 → 印度城市分类发布广告 | 印度 |
| 372 | **PostKarlo** | 注册 → 印度分类发布广告 | 印度 |
| 373 | **SunnySellz** | 注册 → 买卖分类发布广告 | 全球 |
| 374 | **Gezow** | 注册 → 分类发布广告 | 全球 |
| 375 | **LeslieClassified** | 注册 → 分类发布广告 | 全球 |
| 376 | **FamilyAndLand** | 注册 → 家庭/土地分类发布广告 | 全球 |
| 377-384 | MuzaffarnagarBN / KissanKings / CommonBazaar / TheIthum / EclipseAds / JeeoLists / EasyTradeWay / ApniChhat | 注册 → 分类发布广告 | 印度/非洲 |
| 385-388 | AckLists / Dial2Day / LetzDeal / KikList | 注册 → 分类发布广告 | 全球 |

### Nofollow 分类广告站

| # | 网站 | 地区 |
|---|------|------|
| 389 | Hoobly | 全球 |
| 390 | ClassifiedAds.com | 全球 |
| 391-399 | FreeAdsTime / NowShenzhen / AdsAnsar / Global-Free-Classified-Ads / FreeAd1.net / AdfreePosting / NearBuy.com.ng / MowerTuneup | 各地区 |

---

# 十四、Product Launch 产品发布类

> 通用方法：提交产品信息（名称、描述、截图、网站链接） → 平台审核后展示。大部分需审核。

## 400. Product Hunt (producthunt.com)

**DA**: 90+ | **费用**: 免费 | **类型**: 产品发布

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 提交产品 | 注册 → Submit → 填写产品信息+链接 | 待验证 | 高 |

### 操作步骤

1. 注册 https://producthunt.com
2. 提交产品（需 Hunter 推荐或自行提交）
3. 填写产品名/Tagline/描述/截图/链接
4. 选择发布日期参与当日排名

### Tips

- 建议提前联络 Hunter 推荐
- 准备好投票社群
- PST 午夜后发布效果最佳

## 401. Hacker News (news.ycombinator.com)

**DA**: 90+ | **费用**: 免费 | **类型**: 创业新闻

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| Show HN 发帖 | 注册 → 用 "Show HN:" 前缀发帖 | 待验证 | 高 |
| About 字段 | 个人资料 → About 填写链接 | 待验证 | 中 |

### 操作步骤

1. 注册 https://news.ycombinator.com
2. 先养号积累 karma
3. 用 "Show HN: 产品名" 格式发帖
4. 标题含链接

### Tips

- 先养号再发，纯广告会被 flag
- 技术社区，内容需有技术含量

### 其他产品发布平台

| # | 网站 | 入口 | 备注 |
|---|------|------|------|
| 402 | AlternativeTo | 注册 → 提交软件作为替代品 | |
| 403 | BetaList | 提交 Beta 产品等审核 | |
| 404 | SaaSHub | 提交 SaaS 替代品 | |
| 405-438 | StackShare / EU-Startups / SaaSWorthy / AppsZoom / StartupStash / SideProjectors / FeedMyApp / StartupRanking / MakerLog / BetaPage / StartupBase / BetaBound / LaunchingNext / PreFundia / TheStartupPitch / StartupBuffer / StartupLister / GetWorm / StartupCollections / Betafy / Launched.io / AllStartups / StartupInspire / Fiddy / SideProjects.net / PromoteProject / BigStartups / Owwly / TrendyStartups / AppRater / GrowingPage / ToolFinder / Dealify / GetApp | 注册 → 提交产品信息和链接 | 大部分免费，需审核 |

---

# 十五、Crowdfunding 众筹类

> 通用方法：创建众筹项目 → 项目描述中包含网站链接。门槛最高，需真实筹资计划。

## 439. Kickstarter (kickstarter.com)

**DA**: 93 | **费用**: 免费创建/成功抽佣 5% | **类型**: 众筹

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 项目页面链接 | 注册创作者 → 创建项目 → 描述放链接 | 待验证 | 高 |

### 操作步骤

1. 注册 https://kickstarter.com
2. 创建项目（设定筹资目标、奖励层级、时间线）
3. 项目描述中放入网站链接
4. 审核通过后发布

### Tips

- 需要真实的筹资计划
- 平台抽取 5% 佣金 + 支付手续费

## 440. Indiegogo (indiegogo.com)

**DA**: 90+ | **费用**: 免费创建/成功抽佣 5% | **类型**: 众筹

### 可用方法

| 方法 | 入口 | 链接属性 | SEO价值 |
|------|------|----------|---------|
| 项目页面链接 | 注册 → 创建众筹活动 → 描述放链接 | Nofollow | 中 |

### 操作步骤

1. 注册 https://indiegogo.com
2. 创建众筹活动（支持固定目标和弹性目标）
3. 项目页添加网站链接
4. 提交审核

### Dofollow 众筹平台

| # | 网站 | 入口 | 链接属性 |
|---|------|------|----------|
| 441 | **Ulule** (ulule.com) | 注册 → 创建众筹项目 → 描述放链接 | **Dofollow** |
| 442 | **SeedAndSpark** (seedandspark.com) | 注册 → 创建影视众筹 → 描述放链接 | **Dofollow** |
| 443 | **StartupXplore** (startupxplore.com) | 注册 → 创建公司页面 → 网站链接 | **Dofollow** |

### Nofollow 众筹平台

| # | 网站 | 链接属性 |
|---|------|----------|
| 444 | Republic (republic.com) | Nofollow |

