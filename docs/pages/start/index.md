# 开始使用主题

## 项目仓库

<div class="grid cards" markdown>

-   ![图标](../../images/icon.png){#ico .no-zoom} <name>material-mkdocs-theme</name>

    ***

    一款适用于 :simple-materialformkdocs: Material-Mkdocs 的极简风格主题。
    [查看项目 :octicons-chevron-right-12:](https://github.com/GaoZQi/material-mkdocs-theme){#right .md-button .md-button--primary}

</div>

## 下载主题

首先，创建一个新的 MkDocs 项目，或者使用现有的 MkDocs 项目。目录结构如下所示：

    ├─docs
    │  └─...
    └─site

在项目目录下，选择一个合适的文件夹来存放主题文件，例如 `theme` 文件夹。然后，将主题文件下载解压到该文件夹中。

    ├─docs
    │  ├─...
    │  └─theme
    │      ├─css
    │      └─js
    └─site

或者，在指定目录下，使用以下命令直接克隆主题文件：

```bash
git clone git@github.com:GaoZQi/material-mkdocs-theme.git
```

如果想要持续接收主题更新，推荐使用下面的命令：

```bash
git submodule add -b main git@github.com:GaoZQi/material-mkdocs-theme.git .\\docs\\theme
```

## 配置主题

在 `mkdocs.yml` 文件中，添加以下配置：

```yaml
theme:
    palette:
        scheme: auto

extra_css:
    - theme/css/import.css

extra_javascript:
    - theme/js/zoom.js
```

其中，`scheme` 必须设置为 `auto` 确保主题支持深色模式。

完成配置后，运行以下命令启动 MkDocs 服务器：

```bash
mkdocs serve
```

如果配置无误，可以看到主题已经成功应用。
