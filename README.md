---
title: Lorem ipsum
author: dummy
description: this block is YAML front matters
---

# Typora-Theme-Neumorphism

- 新拟态风格。
- 包含字体文件（中文字体禁止用于商业，英文字体为开源字体）
- 仅包含基本 Markdown 功能，并未使用技巧来增强 Markdown。后期可能会视情况添加更多的技巧来增强相关功能。
- 默认提供 亮暗 两种模式。
- 并未针对 PDF 导出做配适性优化。
- 本主题的 CSS 文件由 Less 文件导出。

# 技巧

请注意，以下所列明的技巧或者是依赖于特定的 css 文件，或者是依赖于特定的 js 文件。一些技巧可能只能在特定主题中使用，在进行迁移文档时，需要注意可能在其他软件上无法使用或者展示。

## 修改鼠标样式

本技巧来源于 [用原生 JS 写一款乖巧的鼠标指针特效](https://zhuanlan.zhihu.com/p/351951477)。

具体操作需要修改程序本体，在程序升级之后，需要重新进行设计。

1. 为 typora 注入 js 文件：
   - 复制 `cursor.js`内的代码
   - 粘贴到 typora 的 `index.html` 文件代码中`</body>`之前（可以直接检索）
     - 在 macOS 中，该文件位于 `/Applications/Typora.app/Contents/Resources/TypeMark/index.html`
     - 在 Windows 中，该文件位于`C:\Program Files\Typora\resources\window.html`
1. 重启软件即可

## 图片的技巧

1. 快速调节照片大小：将下方的任意一个位置的数字调整为自己想要缩放的大小即可。

    <center><var>方法： <code>![照片名称 数字](照片地址 "数字")</code> </var></center> 

    <center><var>例如：调整为 50%大小<code>![照片名称 50](照片地址 "50")</code> </var></center> 

    > 注意：默认设定的缩放大小以 5 为步值，即：0，5，10，15……

1. 需要注意的是无法调整照片为行内元素。

## HTML 元素引入

1. 可以通过 `<var> </var>`元素来引入下面的样式：
   - <var> 该元素的本来语义是定义变量。</var>

## 目前已知问题

1. [【issue 5】](https://github.com/Soanguy/Typora-Theme-Neumorphism/issues/5) 在导出为 HTML 文件时，四级标题中如果含有符号的话，将不能如期的显示动画。

# 排版示例

In [publishing](https://www.wikiwand.com/en/Publishing) and [graphic design](https://www.wikiwand.com/en/Graphic_design), **lorem ipsum** (derived from Latin *dolorem ipsum*, translated as "pain itself") is a [filler text](https://www.wikiwand.com/en/Filler_text) commonly used to demonstrate the graphic elements of a document or visual presentation. [^1]

## Example text

A common form of *lorem ipsum* reads:

> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

----

Inline styles support **strong**, *Emphasis*, `code`, <u>underline</u>, ~~strikethrough~~, :haha:, $\LaTeX$, X^2^, H~2~O, ==highlight==, [Link](typora.io), and image:

![img](https://i.imgur.com/RGLj3oV.jpg)

Block level contains:

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

| Left-Aligned  |     Center Aligned     | Right Aligned |
| :------------ | :--------------------: | ------------: |
| col 3 is      | <u>some wordy text</u> |         $1600 |
| col 2 is      |        centered        |           $12 |
| zebra stripes |        are neat        |            $1 |

1. ordered list item 1.
2. ordered list item 2.
   + sub-unordered list item 1.
   + sub-unordered list item 2.
     + [ ] something is DONE.
     + [ ] something is not TODO.

```html
<!DOCTYPE html>
<html>
<body>

<h1>The *= Operator</h1>
  
<p id="demo"></p>

<script>
var x = 10;
x *= 5;
document.getElementById("demo").innerHTML = x;
</script>

</body>
</html>
```

[TOC]

[^1]: *Forked* from https://en.wikipedia.org/wiki/Lorem_ipsum
