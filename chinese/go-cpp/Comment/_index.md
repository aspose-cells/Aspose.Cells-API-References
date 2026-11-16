---
title: "Comment 类"
linktitle: "Comment"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Comment 类。封装在 Go 中表示注释的对象。"
type: docs
weight: 200
url: /zh/go-cpp/comment/
---

## Comment class

封装表示单元格批注的对象。

```go

type Comment struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetAuthor](./getauthor/) | 获取并设置原始评论作者的 Name。 |
| [SetAuthor](./setauthor/) | 获取并设置原始评论作者的 Name。 |
| [GetCommentShape](./getcommentshape/) | 获取一个 Shape 对象，表示附加到指定评论的形状。 |
| [GetRow](./getrow/) | 获取评论的行索引。 |
| [GetColumn](./getcolumn/) | 获取评论的列索引。 |
| [IsThreadedComment](./isthreadedcomment/) | 指示此评论是否为线程式评论。 |
| [GetThreadedComments](./getthreadedcomments/) | 获取线程式评论的列表； |
| [GetNote](./getnote/) | 表示评论的内容。 |
| [SetNote](./setnote/) | 表示评论的内容。 |
| [GetHtmlNote](./gethtmlnote/) | 获取并设置包含此评论中数据和某些格式的 html 字符串。 |
| [SetHtmlNote](./sethtmlnote/) | 获取并设置包含此评论中数据和某些格式的 html 字符串。 |
| [GetFont](./getfont/) | 获取评论的字体。 |
| [FormatCharacters](./formatcharacters/) | 使用字体设置格式化某些字符。 |
| [Characters](./characters/) | 返回一个 Characters 对象，表示评论文本中一段字符范围。 |
| [GetRichFormattings](./getrichformattings/) | 返回所有 Characters 对象，表示评论文本中一段字符范围。 |
| [IsVisible](./isvisible/) | 表示评论是否可见。 |
| [SetIsVisible](./setisvisible/) | 表示评论是否可见。 |
| [GetTextOrientationType](./gettextorientationtype/) | 获取并设置评论的文本方向类型。 |
| [SetTextOrientationType](./settextorientationtype/) | 获取并设置评论的文本方向类型。 |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | 获取并设置评论的文本水平对齐类型。 |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | 获取并设置评论的文本水平对齐类型。 |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | 获取并设置评论的文本垂直对齐类型。 |
| [SetTextVerticalAlignment](./settextverticalalignment/) | 获取并设置评论的文本垂直对齐类型。 |
| [GetAutoSize](./getautosize/) | 指示是否根据内容自动调整评论的大小。注意：在某些特殊情况下（例如 Mac 环境），此设置可能无效。如果此设置无效，请改用 FitToTextSize()。 |
| [SetAutoSize](./setautosize/) | 指示是否根据内容自动调整评论的大小。注意：在某些特殊情况下（例如 Mac 环境），此设置可能无效。如果此设置无效，请改用 FitToTextSize()。 |
| [GetHeightCM](./getheightcm/) | 表示评论的高度，单位为厘米。 |
| [SetHeightCM](./setheightcm/) | 表示评论的高度，单位为厘米。 |
| [GetWidthCM](./getwidthcm/) | 表示评论的宽度，单位为厘米。 |
| [SetWidthCM](./setwidthcm/) | 表示评论的宽度，单位为厘米。 |
| [GetWidth](./getwidth/) | 表示评论的宽度，单位为像素。 |
| [SetWidth](./setwidth/) | 表示评论的宽度，单位为像素。 |
| [GetHeight](./getheight/) | 表示评论的高度，单位为像素。 |
| [SetHeight](./setheight/) | 表示评论的高度，单位为像素。 |
| [GetWidthInch](./getwidthinch/) | 表示评论的宽度，单位为英寸。 |
| [SetWidthInch](./setwidthinch/) | 表示评论的宽度，单位为英寸。 |
| [GetHeightInch](./getheightinch/) | 表示评论的高度，单位为英寸。 |
| [SetHeightInch](./setheightinch/) | 表示评论的高度，单位为英寸。 |
