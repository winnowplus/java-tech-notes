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
