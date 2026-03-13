# GitHub Markdown 语法指南

## 目录
- [标题](#标题)
- [文本样式](#文本样式)
- [列表](#列表)
- [代码](#代码)
- [链接与图片](#链接与图片)
- [引用](#引用)
- [表格](#表格)
- [任务列表](#任务列表)
- [删除线](#删除线)
- [分割线](#分割线)
- [表情符号](#表情符号)
- [脚注](#脚注)

## 标题

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

## 文本样式

- **粗体文本**: `**粗体文本**` 或 `__粗体文本__`
- *斜体文本*: `*斜体文本*` 或 `_斜体文本_`
- **粗斜体文本**: `***粗斜体文本***`
- `行内代码`: 使用反引号 \`code\`
- ~~删除线~~: `~~删除线~~`

## 列表

### 无序列表
```markdown
- 项目 1
- 项目 2
  - 嵌套项目 2.1
  - 嵌套项目 2.2
- 项目 3
```

效果：
- 项目 1
- 项目 2
  - 嵌套项目 2.1
  - 嵌套项目 2.2
- 项目 3

### 有序列表
```markdown
1. 第一项
2. 第二项
   1. 嵌套第一项
   2. 嵌套第二项
3. 第三项
```

效果：
1. 第一项
2. 第二项
   1. 嵌套第一项
   2. 嵌套第二项
3. 第三项

## 代码

### 行内代码
使用 \`code\` 来标记行内代码，例如：`console.log('Hello, World!')`

### 代码块
使用三个反引号来创建代码块，并可以指定语言：

\`\`\`javascript
function greet(name) {
    console.log(`Hello, ${name}!`);
}

greet('GitHub');
\`\`\`

效果：
```javascript
function greet(name) {
    console.log(`Hello, ${name}!`);
}

greet('GitHub');
```

## 链接与图片

### 链接
```markdown
[链接文本](https://github.com)
[带标题的链接](https://github.com "GitHub 主页")
```

效果：
[GitHub](https://github.com)

### 图片
```markdown
![替代文本](图片URL)
![替代文本](图片URL "图片标题")
```

示例：
![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

### 带链接的图片
```markdown
[![图片替代文本](图片URL)](链接URL)
```

## 引用

```markdown
> 这是一级引用
> 
> > 这是二级引用
> > 
> > > 这是三级引用
```

效果：
> 这是一级引用
> 
> > 这是二级引用

## 表格

```markdown
| 左对齐 | 居中 | 右对齐 |
| :--- | :---: | ---: |
| 左侧内容 | 中间内容 | 右侧内容 |
| 单元格 | 单元格 | 单元格 |
```

效果：

| 左对齐 | 居中 | 右对齐 |
| :--- | :---: | ---: |
| 左侧内容 | 中间内容 | 右侧内容 |
| 单元格 | 单元格 | 单元格 |

## 任务列表

```markdown
- [x] 已完成任务
- [ ] 未完成任务
- [ ] 另一个未完成任务
```

效果：
- [x] 已完成任务
- [ ] 未完成任务
- [ ] 另一个未完成任务

## 删除线

```markdown
~~这段文本被删除了~~
```

效果：
~~这段文本被删除了~~

## 分割线

使用三个或更多的 `-`、`*` 或 `_`：

```markdown
---
***
___
```

效果：

---

***

___

## 表情符号

GitHub 支持 emoji 表情符号，使用 `:emoji_name:` 格式：

```markdown
:smile: :heart: :rocket: :thumbsup: :octocat:
```

效果：
:smile: :heart: :rocket: :thumbsup: :octocat:

## 脚注

```markdown
这是一个脚注引用[^1]

[^1]: 这是脚注的内容。
```

效果：
这是一个脚注引用[^1]

[^1]: 这是脚注的内容。

## 转义字符

使用反斜杠 `\` 来转义特殊字符：

```markdown
\*这不是斜体\*
\# 这不是标题
```

效果：
\*这不是斜体\*
\# 这不是标题

## HTML 标签

Markdown 也支持部分 HTML 标签：

```html
<div align="center">
  <strong>居中加粗文本</strong>
</div>

<details>
<summary>点击展开</summary>

这里是隐藏的内容。

</details>
```

效果：

<div align="center">
  <strong>居中加粗文本</strong>
</div>

<details>
<summary>点击展开</summary>

这里是隐藏的内容。

</details>

## 快捷键

可以使用 `<kbd>` 标签来表示键盘按键：

```html
按 <kbd>Ctrl</kbd> + <kbd>C</kbd> 复制
```

效果：
按 <kbd>Ctrl</kbd> + <kbd>C</kbd> 复制

## 数学公式

GitHub 支持使用 LaTeX 语法显示数学公式：

行内公式：`$E=mc^2$`

效果：$E=mc^2$

块级公式：

```markdown
$$
\frac{\partial f}{\partial x} = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}
$$
```

效果：
$$
\frac{\partial f}{\partial x} = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}
$$

## 提示框 (GitHub 特有)

GitHub 支持特殊的提示框语法：

```markdown
> [!NOTE]
> 这是一个提示

> [!WARNING]
> 这是一个警告

> [!IMPORTANT]
> 这是重要信息
```

效果：

> [!NOTE]
> 这是一个提示

> [!WARNING]
> 这是一个警告

> [!IMPORTANT]
> 这是重要信息

---

## 参考资源

- [GitHub Markdown 官方文档](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [GitHub 风格的 Markdown 规范](https://github.github.com/gfm/)
- [Emoji 速查表](https://github.com/ikatyang/emoji-cheat-sheet)
