# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Claude Code Skill 插件支持
  - 在 Claude Code 中直接查询 AI 资讯
  - 支持相对日期查询（昨天、前天、今天）
  - 支持绝对日期查询（YYYY-MM-DD）
  - 内置 Claude AI 智能摘要和分类
  - 可选生成精美网页（苹果风/深海蓝/秋日暖阳主题）
  - 友好的用户无数据提示

### Changed
- 邮件通知改为可选配置
- 修复空环境变量导致 SMTP_PORT 转换失败的问题
- 修复邮件未配置时 total_items 未定义的错误

[Unreleased]: https://github.com/geekjourneyx/ai-daily-skill/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/geekjourneyx/ai-daily-skill/releases/tag/v1.0.0

---

## [1.0.0] - 2026-01-15

### Added
- 自动从 smol.ai 获取 AI 资讯
- Claude AI 智能分析分类和摘要提取
- 8 种智能主题配色，根据内容类型自动选择
- 精美 HTML 页面生成，支持响应式设计
- 邮件通知功能（可选配置）
  - 成功通知：包含资讯数量和页面链接
  - 空数据通知：当日无资讯时提醒
  - 错误通知：失败时附带 GitHub Actions 日志链接
- GitHub Actions 定时任务
  - 每天 UTC 02:00（北京时间 10:00）自动运行
  - 支持手动触发
  - 自动部署到 GitHub Pages
- 资讯智能分类（模型发布、产品动态、研究论文、工具框架、融资并购、行业事件）
- 索引页面，按日期倒序展示所有日报
- 关键词提取和标签展示

### Configuration
- 支持 8 种主题配色：柔和蓝色、深靛蓝、优雅紫色、清新绿色、温暖橙色、玫瑰粉色、冷色青绿、中性灰色
- 支持通过环境变量自定义 RSS 源
- 支持通过环境变量配置 SMTP 邮件通知

### Documentation
- 完整的 README.md 使用文档
- 常见问题（FAQ）章节
- 本地开发指南

[Unreleased]: https://github.com/geekjourneyx/ai-daily-skill/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/geekjourneyx/ai-daily-skill/releases/tag/v1.0.0
