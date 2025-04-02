# 拓展组件

## 超链接

具有线条动画的超链接，使用方法如下：

```markdown
[超链接](https://example.com)
```

!!! tip "移除线条动画"

    如果不想使用线条动画，可以添加`#no-underline`来移除该功能。

    ```markdown
    [超链接](https://example.com){ #no-underline}
    ```

### 效果展示

[超链接](https://example.com)

## 图片缩放（已移除）

在点击图片时，图片会放大显示。

### 使用方法

使用方式，在`mkdocs.yml`中添加下面配置：

```yaml
extra_javascript:
    - ./docs/theme/js/zoom.js
```

!!! tip "屏蔽放大功能"

    如果不想使用图片缩放功能，可以添加`.no-zoom`来屏蔽该功能。

    ```markdown
    ![图片描述](https://example.com/image.png){ .no-zoom}
    ```

## 图标

快速添加圆形图标，使用方法如下：

```markdown
![图标](https://example.com/icon.png){#ico}
```

### 效果展示

![GaoZQi](https://avatars.githubusercontent.com/u/62362150?v=4 "GaoZQi"){#ico .off-glb}

## 提示块

添加两种提示块，使用方法如下：

```markdown
!!! caution "提示块标题"

    提示块内容
```

```markdown
!!! important "提示块标题"

    提示块内容
```

### 效果展示

!!! caution

    caution可以用来表示警告、注意事项等信息。

!!! important

    important可以用来表示重要信息、提示等内容。

## 按钮

为按钮添加了几张方位和长度 id，使用方法如下：

```markdown
[按钮](https://example.com){#right .md-button}
```

```markdown
markdown
[按钮](https://example.com){#width-left .md-button}
```

```markdown
[按钮](https://example.com){#width .md-button}
```

```markdown
[按钮](https://example.com){#width-pic .md-button}
```

!!! tip "按钮说明"

    - `#right`：按钮右侧对齐。
    - `#width-left`：文字左侧对齐。
    - `#width`：文字居中，宽度为100%。
    - `#width-pic`：文字居中，宽度图片相同，模糊效果，位于图片底部，需要配合图片卡片使用。

### 效果展示

[按钮](#_5){#right .md-button}

[按钮](#_5){#width-left .md-button}

[按钮](#_5){#width .md-button}

## 图片卡片

以固定高度展示图片，使用方法如下：

```markdown
![图片](https://example.com/image.png){#card-pic}
```

### 效果展示

![图片](../../images/icon.png){#card-pic}

[按钮](#_5){#width-pic .md-button}
