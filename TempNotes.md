# Temp Notes

## MkDocs 项目结构

```text
root/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions 自动部署配置
├── docs/
│   └── index.md                # 站点首页
├── mkdocs.yml                  # MkDocs 配置文件
└── README.md                   # 仓库说明文件
```

## MkDocs 主题

| 排名 | 主题名称 | 特点 | 链接（可查看效果图） |
| :---: | :--- | :--- | :--- |
| 1 | Material for MkDocs | 目前最流行、功能最丰富的主题。支持暗色模式、多语言、搜索建议、代码复制、Mermaid 图表等。社区活跃，插件生态完善。 | [官方文档](https://squidfunk.github.io/mkdocs-material/)（首页即演示） |
| 2 | Read the Docs | MkDocs 内置主题之一。风格简洁、经典，适合技术文档。支持导航折叠、搜索等基础功能。 | [官方示例](https://mkdocs.readthedocs.io/en/stable/) |
| 3 | MkDocs 默认主题 | MkDocs 内置的默认主题。极简风格，无多余装饰，适合快速搭建。 | [官方示例](https://www.mkdocs.org/) |
| 4 | Windmill | 一个轻量、干净的第三方主题。设计风格偏向现代、扁平，适合个人博客或小型项目文档。 | [GitHub 仓库](https://github.com/gristlabs/mkdocs-windmill)（含截图） |
| 5 | Bootswatch | 基于 Bootstrap 的主题集合。提供多种配色方案（如 Cerulean、Cosmo、Flatly 等），适合喜欢 Bootstrap 风格的用户。 | [MkDocs Bootswatch](https://mkdocs.github.io/mkdocs-bootswatch/)（含在线演示） |
| 6 | Cinder | 一个简洁、响应式的第三方主题。风格类似 Read the Docs，但更轻量。 | [GitHub 仓库](https://github.com/chrissimpkins/cinder)（含截图） |
| 7 | Alabaster | 一个干净、优雅的第三方主题。最初为 Sphinx 设计，后移植到 MkDocs。 | [PyPI 页面](https://pypi.org/project/mkdocs-alabaster/)（含截图） |

## MkDocs 插件增强

| 插件  | 功能  | 需要特殊语法吗？ |
| :---: | :---: |::---:|
| `search` | 全文搜索 | ❌ 不需要 |
| `awesome-pages` | 自动生成侧边栏导航 | ❌ 不需要（可配 `.pages` 文件，但不是必须的） |
| `minify` | 压缩 HTML/CSS/JS，加快加载速度 | ❌ 不需要 |
| `git-revision-date` | 显示文件最后修改时间 | ❌ 不需要 |
| `git-committers` | 显示文件的贡献者 | ❌ 不需要 |
| `tags` | 自动生成标签页 | ❌ 不需要（需在 Markdown 文件头部加 metadata，但语法是标准 YAML） |

如果你追求极致的语义准确，选 ⚓；如果你追求最广泛的认知度，选 🔗；如果你追求最干净、最技术范，选 `#`
