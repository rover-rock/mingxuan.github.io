# 我的个人日记网站

这是一个基于 Jekyll 构建的个人日记网站，用于记录生活点滴、学习心得和个人感悟。

## 📖 网站特色

- **简洁优雅的设计**：采用现代化的响应式设计，在各种设备上都有良好的阅读体验
- **分类标签系统**：支持按分类和标签对日记进行组织
- **心情天气记录**：每篇日记可以记录当时的心情和天气
- **归档功能**：提供按时间归档的日记浏览方式
- **搜索导航**：清晰的导航结构，方便查找历史日记

## 🗂️ 项目结构

```
.
├── _config.yml          # Jekyll 配置文件
├── _layouts/            # 页面模板
│   ├── default.html     # 默认模板
│   └── post.html        # 日记文章模板
├── _posts/              # 日记文章目录
│   ├── 2025-01-15-我的第一篇日记.md
│   └── 2025-01-10-学习编程的一天.md
├── assets/              # 静态资源
│   └── css/
│       └── style.css    # 主样式文件
├── index.md             # 首页
├── archive.html         # 归档页面
├── categories.html      # 分类页面
├── tags.html           # 标签页面
├── about.html          # 关于页面
├── Gemfile             # Ruby 依赖配置
└── README.md           # 项目说明
```

## ✍️ 如何写日记

在 `_posts` 目录下创建新的 Markdown 文件，文件名格式为：`YYYY-MM-DD-title.md`

示例日记格式：

```markdown
---
layout: post
title: "日记标题"
date: 2025-01-15 20:30:00 +0800
categories: 日记
tags: [生活, 感悟]
mood: 开心
weather: 晴朗
---

## 今天的天气
描述今天的天气情况...

## 今天做了什么
- 列出今天的主要活动
- 记录重要的事件

## 今天的感悟
分享你的思考和感悟...

## 明天的计划
- [ ] 待办事项1
- [ ] 待办事项2
```

### Front Matter 字段说明

- `layout`: 使用的模板（通常为 `post`）
- `title`: 日记标题
- `date`: 发布时间（格式：YYYY-MM-DD HH:MM:SS +0800）
- `categories`: 分类（如：日记、学习、工作等）
- `tags`: 标签数组（用于更细致的分类）
- `mood`: 心情（可选字段）
- `weather`: 天气（可选字段）

## 🚀 本地开发

1. 确保你已安装 Ruby 和 Bundler
2. 克隆项目到本地
3. 安装依赖：
   ```bash
   bundle install
   ```
4. 启动本地服务器：
   ```bash
   bundle exec jekyll serve
   ```
5. 在浏览器中访问 `http://localhost:4000`

## 🌐 部署到 GitHub Pages

1. 将项目推送到 GitHub 仓库
2. 在仓库设置中启用 GitHub Pages
3. 选择 GitHub Actions 作为构建方式
4. 确保 `.github/workflows/jekyll.yml` 工作流文件存在
5. 每次推送代码后，网站会自动构建和部署

## 📝 写作建议

- **保持规律**：尝试养成定期写日记的习惯
- **真实记录**：诚实地记录你的想法和感受
- **分类标签**：合理使用分类和标签，便于后续查找
- **添加细节**：记录具体的时间、地点、人物等细节
- **反思总结**：不仅记录事件，更要记录你的思考和感悟

## 🎨 自定义

你可以通过以下方式个性化你的日记网站：

- 修改 `_config.yml` 中的网站信息
- 在 `assets/css/style.css` 中调整样式
- 更新 `about.html` 中的个人信息
- 添加新的页面和功能

## 📊 统计信息

网站会自动生成：
- 日记总数统计
- 分类和标签统计
- 按月份的归档
- RSS 订阅源

## 🔗 相关链接

- [Jekyll 官方文档](https://jekyllrb.com/)
- [GitHub Pages 文档](https://pages.github.com/)
- [Markdown 语法指南](https://www.markdownguide.org/)

---

开始你的日记之旅吧！记录生活，分享思考，让文字成为时光的见证。