# AI Learn Hub 项目

欢迎来到 AI Learn Hub 项目！这是一个帮助你学习和探索 AI 的网站。

## 项目目标

创建一个简洁、易于访问的网站，用于分享 AI 学习资源和心得。

## 文件结构

-   `index.html`: 这是网站的主页面（首页）。目前它包含一个简单的欢迎标题，并且已经集成了 Google Analytics 和 Plausible 的网站统计功能。

## 页面说明

### 首页 (`index.html`)

-   **用途**: 作为网站的入口，向访问者展示欢迎信息。
-   **布局**: 目前是一个非常基础的上下结构，包含一个主标题和一个段落。
-   **代码说明**:
    -   `<head>` 部分：包含了网站的元信息（比如编码格式、标题）以及用于追踪网站流量的分析工具：
        - **Google Analytics (GA4)**: 使用追踪ID `G-VYEBQ2KVHH`，提供详细的网站访问数据分析
        - **Plausible Analytics**: 面向隐私保护的轻量级分析工具，域名为 `ailearnhub.app`
        这些分析工具都是匿名的，只会统计网站访问量和基本行为数据，不会收集个人隐私信息。
    -   `<body>` 部分：包含了网站上所有可见的内容，比如文字、图片等。

## SEO优化说明

### 已修复的问题（2025-01-12）

1. **域名大小写统一**：
   - 将所有meta标签和canonical URL中的`aiLearnhub.APP`统一改为小写`ailearnhub.app`
   - 修复了可能导致Google认为存在重复页面的问题

2. **添加了SEO基础文件**：
   - `robots.txt`：指导搜索引擎爬虫如何抓取网站
   - `sitemap.xml`：帮助搜索引擎发现和索引页面

3. **结构化数据优化**：
   - 更新了JSON-LD结构化数据中的URL为统一的小写格式

### Google Search Console问题解决

针对显示的"网页未被编入索引的原因"问题：
- **备用网页（有适当的规范标记）**：通过统一域名大小写解决
- **网页会自动重定向**：确保canonical URL指向正确的域名格式

### 建议的后续操作

1. 重新提交sitemap到Google Search Console
2. 请求重新索引主页面
3. 监控索引状态变化

### Sitemap问题修复（2025-01-12 更新）

**问题**：Google Search Console显示"Sitemap 是 HTML"错误

**解决方案**：
1. 更新了sitemap.xml，添加了更完整的XML Schema声明
2. 创建了.htaccess文件，确保：
   - XML文件以正确的MIME类型(`application/xml`)提供服务
   - 启用了Gzip压缩优化性能
   - 设置了合适的缓存策略

**验证方法**：
- 直接访问 `https://ailearnhub.app/sitemap.xml` 确认显示为XML格式
- 在Google Search Console中重新测试sitemap

## 后续计划

-   丰富首页内容。
-   添加新的页面，例如"学习资源"和"关于我"。
-   设计美观的 CSS 样式，让网站更好看。
-   持续监控SEO表现。

---
*由你的 AI 高级工程师创建* 