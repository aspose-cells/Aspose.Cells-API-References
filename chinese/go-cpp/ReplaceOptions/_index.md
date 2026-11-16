---
title: "ReplaceOptions 类"
linktitle: "ReplaceOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ReplaceOptions 类。封装表示 Go 中 replaceoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/replaceoptions/
---

## ReplaceOptions class

表示替换选项。

```go

type ReplaceOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewReplaceOptions](./newreplaceoptions/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetCaseSensitive](./getcasesensitive/) | 指示搜索的字符串是否区分大小写。 |
| [SetCaseSensitive](./setcasesensitive/) | 指示搜索的字符串是否区分大小写。 |
| [GetMatchEntireCellContents](./getmatchentirecellcontents/) | 指示是否匹配整个单元格内容 |
| [SetMatchEntireCellContents](./setmatchentirecellcontents/) | 指示是否匹配整个单元格内容 |
| [GetRegexKey](./getregexkey/) | 指示搜索的键是否为正则表达式。如果为 true，则搜索的键将被视为正则表达式。 |
| [SetRegexKey](./setregexkey/) | 指示搜索的键是否为正则表达式。如果为 true，则搜索的键将被视为正则表达式。 |
| [GetFontSettings](./getfontsettings/) | 替换文本的富格式设置。 |
| [SetFontSettings](./setfontsettings/) | 替换文本的富格式设置。 |
| [GetStyleFlags](./getstyleflags/) | 获取并设置应用字体设置的标志。 |
| [SetStyleFlags](./setstyleflags/) | 获取并设置应用字体设置的标志。 |
