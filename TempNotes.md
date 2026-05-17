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

[mkdocs-gallery](https://pawamoy.github.io/mkdocs-gallery/) 陈列了几乎所有主题，其中值得关注的有：

|   内置主题    | 适用     | ShowCase                                                           |
| :-----------: | :------- | :----------------------------------------------------------------- |
|    MkDocs     | 默认     | <https://mkdocs.readthedocs.io/en/stable/user-guide/installation/> |
| Read the Docs | API 文档 | <https://docs.readthedocs.com/platform/stable/>                    |

| 第三方主题 | 适用             | ShowCase                                       |
| :--------: | :--------------- | :--------------------------------------------- |
|  Material  |                  | <https://squidfunk.github.io/mkdocs-material/> |
|  Windmill  | 轻量 简洁风      | <https://gristlabs.github.io/mkdocs-windmill/> |
| Bootswatch | Bootstrap 风格   | <https://mkdocs.github.io/mkdocs-bootswatch/>  |
|   Cinder   | 类 Read the Docs | <https://sourcefoundry.org/cinder/>            |

```yml
# ---------- 主题配置 ----------
theme:
  name: material                           # 使用 Material for MkDocs 主题
  language: zh                             # 界面语言设为中文
  palette:
    - scheme: default
      primary: blue grey
      accent: teal
      toggle:
        icon: material/weather-night      # 月亮图标，点击切换到暗色
        name: 切换至暗色模式
    - scheme: slate
      primary: indigo
      accent: teal
      toggle:
        icon: material/weather-sunny      # 太阳图标，点击切换到亮色
        name: 切换至亮色模式
  features:
    - navigation.tabs                      # 顶部导航标签页
    - navigation.sections                  # 侧边栏按章节分组
    - navigation.expand                    # 侧边栏默认展开
    - navigation.top                       # 页面右下角返回顶部按钮
    - search.suggest                       # 搜索框显示建议
    - search.highlight                     # 搜索结果高亮
    - content.code.copy                    # 代码块右上角显示复制按钮
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
