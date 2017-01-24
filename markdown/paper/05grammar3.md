# MarkDown 语法 3

## 表格

表格不在 MarkDown 的规范里，但是很多解释器都支持表格。尤其是 Github 使用的 **GFM** 也是支持表格的。

MarkDown用横线（`-`）和竖线（`|`）来制作表格。并使用冒号来控制表格的对齐，如下面的例子所示：

    | 这         | 是       | 表头      |
    | ---------- |:--------:| -------- :|
    | 左侧对齐   | 居中对齐 | 右侧对齐  |
    | 左侧对齐   | 居中对齐 | 右侧对齐  |

上面的表格显示效果如下：

| 这         | 是       | 表头         |  
| ------------ |:--------:| ------------ :|  
| 左侧对齐 | 居中对齐 | 右侧对齐  |  
| 左侧对齐 | 居中对齐 | 右侧对齐  |  

这里有几个要点：

* 每个单元格至少需要三个横线来间隔，冒号算作一个横线。
* 外侧的竖线（`|`）可以没有。
* 单元格里可以使用 MarkDown 语法。

这就意味着，你可以按照下面的方式来编写表格：

    Markdown | Less | Pretty
    --- | --- | ---
    *Still* | `renders` | **nicely**

虽然上面的代码看上去不美观，但是表格可以正常显示：

Markdown | Less | Pretty  
--- | --- | ---  
*Still* | `renders` | **nicely**

## 水平分隔线

有时我们需要将信息分隔开。在 HTML 中我们使用 `<hr>` 标记，这个标记是两个单词的首字母缩写：_**h**orizontal **r**ule_。

MarkDown 中添加水平分隔线毫无难度。只需要输入三个横线（星号或下划线）即可。

    横线

    ---

    星号

    ***

    下划线

    ___

上面代码的效果如下：

横线

---

星号

***

下划线

___


你应该还记得在 _标题_练习中，三个下划线会让上一行文字变成二级标题。为了避免这种情况，需要在文本和三个下划线中间插入一个空行。

## HTML 语法

如果你想对文档做更多的格式化，而这些格式超出了 MarkDown 的能力范围，你可以使用 HTML 标记，MarkDown 对 HTML 能够很好地兼容。

    <p align="center">可以很好地将文本居中。</p>

这样你就可以得到一个居中的段落。

这个功能非常有用，但是需要小心。HTML 内部的 MarkDown 语法会无效！如果你按下面的方式编写文档：

    <span>Markdown **不能** 正常工作！</span>

它不能正常工作。

### 总结

你可以使用 HTML 编写任何内容：定义列表，嵌入社交网络中的内容，嵌入 YouTube 视频，等等。只需要在你的 MarkDown 文档的合适位置插入 HTML 标记即可。

## 