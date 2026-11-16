---
title: "TextParagraph 类"
linktitle: "文本段落"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TextParagraph 类。封装在 Go 中表示文本段落的对象。"
type: docs
weight: 200
url: /zh/go-cpp/textparagraph/
---

## TextParagraph class

表示文本段落设置。

```go

type TextParagraph struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewTextParagraph](./newtextparagraph/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetBullet](./getbullet/) | 获取项目符号。 |
| [GetType](./gettype/) | 获取文本节点的类型。 |
| [GetLineSpaceSizeType](./getlinespacesizetype/) | 获取并设置段落内部使用的垂直空白量。 |
| [SetLineSpaceSizeType](./setlinespacesizetype/) | 获取并设置段落内部使用的垂直空白量。 |
| [GetLineSpace](./getlinespace/) | 获取并设置段落内部使用的垂直空白量。 |
| [SetLineSpace](./setlinespace/) | 获取并设置段落内部使用的垂直空白量。 |
| [GetSpaceAfterSizeType](./getspaceaftersizetype/) | 获取并设置段落后出现的垂直空白量。 |
| [SetSpaceAfterSizeType](./setspaceaftersizetype/) | 获取并设置段落后出现的垂直空白量。 |
| [GetSpaceAfter](./getspaceafter/) | 获取并设置段落后出现的垂直空白量。 |
| [SetSpaceAfter](./setspaceafter/) | 获取并设置段落后出现的垂直空白量。 |
| [GetSpaceBeforeSizeType](./getspacebeforesizetype/) | 获取并设置段落前出现的垂直空白量。 |
| [SetSpaceBeforeSizeType](./setspacebeforesizetype/) | 获取并设置段落前出现的垂直空白量。 |
| [GetSpaceBefore](./getspacebefore/) | 获取并设置段落前出现的垂直空白量。 |
| [SetSpaceBefore](./setspacebefore/) | 获取并设置段落前出现的垂直空白量。 |
| [GetStops](./getstops/) | 获取制表位列表。 |
| [IsLatinLineBreak](./islatinlinebreak/) | 指定是否可以在不添加连字符的情况下将拉丁单词拆分并换行到下一行。 |
| [SetIsLatinLineBreak](./setislatinlinebreak/) | 指定是否可以在不添加连字符的情况下将拉丁单词拆分并换行到下一行。 |
| [IsEastAsianLineBreak](./iseastasianlinebreak/) | 指定是否可以在不添加连字符的情况下将东亚文字拆分并换行到下一行。 |
| [SetIsEastAsianLineBreak](./setiseastasianlinebreak/) | 指定是否可以在不添加连字符的情况下将东亚文字拆分并换行到下一行。 |
| [IsHangingPunctuation](./ishangingpunctuation/) | 指定标点符号是强制排在同一行文本上，还是放在另一行文本上。 |
| [SetIsHangingPunctuation](./setishangingpunctuation/) | 指定标点符号是强制排在同一行文本上，还是放在另一行文本上。 |
| [GetRightMargin](./getrightmargin/) | 指定段落的右边距。 |
| [SetRightMargin](./setrightmargin/) | 指定段落的右边距。 |
| [GetLeftMargin](./getleftmargin/) | 指定段落的左边距。 |
| [SetLeftMargin](./setleftmargin/) | 指定段落的左边距。 |
| [GetFirstLineIndent](./getfirstlineindent/) | 指定将在段落第一行文本上应用的缩进大小。 |
| [SetFirstLineIndent](./setfirstlineindent/) | 指定将在段落第一行文本上应用的缩进大小。 |
| [GetFontAlignType](./getfontaligntype/) | 确定文本行上实际单词的垂直位置。这涉及字符相对于基线的垂直放置。 |
| [SetFontAlignType](./setfontaligntype/) | 确定文本行上实际单词的垂直位置。这涉及字符相对于基线的垂直放置。 |
| [GetAlignmentType](./getalignmenttype/) | 获取并设置段落的文本水平对齐类型。 |
| [SetAlignmentType](./setalignmenttype/) | 获取并设置段落的文本水平对齐类型。 |
| [GetDefaultTabSize](./getdefaulttabsize/) | 获取并设置此段落中制表符的默认大小。 |
| [SetDefaultTabSize](./setdefaulttabsize/) | 获取并设置此段落中制表符的默认大小。 |
| [GetChildren](./getchildren/) | 获取此段落中的所有文本运行。如果此段落为空，返回段落本身。 |
| [GetStartIndex](./getstartindex/) | 获取字符的起始索引。 |
| [GetLength](./getlength/) | 获取字符的长度。 |
| [GetFont](./getfont/) | 返回此对象的字体。 |
| [SetWordArtStyle](./setwordartstyle/) | 设置预设的 WordArt 样式。 |
| [GetTextOptions](./gettextoptions/) | 返回文本选项。 |
