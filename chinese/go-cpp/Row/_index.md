---
title: "Row 类"
linktitle: "Row"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Row 类。封装在 Go 中表示行的对象。"
type: docs
weight: 200
url: /zh/go-cpp/row/
---

## Row class

表示工作表中的单行。

```go

type Row struct  {
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
| [GetCellByIndex](./getcellbyindex/) | 通过此行的单元格集合中的特定索引获取单元格。 |
| [IsBlank](./isblank/) | 指示该行是否包含任何数据 |
| [Get](./get/) | 获取单元格。 |
| [GetEnumerator](./getenumerator/) | 获取单元格枚举器 |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | 获取一个遍历此行单元格的枚举器。 |
| [GetCellOrNull](./getcellornull/) | 在特定索引处获取单元格或 null。 |
| [IsCollapsed](./iscollapsed/) | 行是否已折叠 |
| [SetIsCollapsed](./setiscollapsed/) | 行是否已折叠 |
| [GetHeight](./getheight/) | 获取和设置以点为单位的行高。 |
| [SetHeight](./setheight/) | 获取和设置以点为单位的行高。 |
| [IsHidden](./ishidden/) | 指示该行是否隐藏。 |
| [SetIsHidden](./setishidden/) | 指示该行是否隐藏。 |
| [GetIndex](./getindex/) | 获取此行的索引。 |
| [GetGroupLevel](./getgrouplevel/) | 获取该行的组级别。 |
| [SetGroupLevel](./setgrouplevel/) | 获取该行的组级别。 |
| [IsHeightMatched](./isheightmatched/) | 指示行高是否匹配工作簿当前的默认字体设置。该属性为 true 时也表示行高为“自动”，即未由用户设置自定义高度值。 |
| [SetIsHeightMatched](./setisheightmatched/) | 指示行高是否匹配工作簿当前的默认字体设置。该属性为 true 时也表示行高为“自动”，即未由用户设置自定义高度值。 |
| [GetStyle](./getstyle/) | 获取此行的样式。 |
| [SetStyle](./setstyle/) | 设置此行的样式。 |
| [GetHasCustomStyle](./gethascustomstyle/) | 指示此行是否具有自定义样式设置（不同于从工作簿继承的默认样式）。 |
| [CopySettings](./copysettings/) | 复制行的设置，例如样式、高度、可见性等。 |
| [GetFirstCell](./getfirstcell/) | 获取该行中的第一个单元格对象。 |
| [GetFirstDataCell](./getfirstdatacell/) | 获取该行中的第一个非空单元格。 |
| [GetLastCell](./getlastcell/) | 获取该行中的最后一个单元格对象。 |
| [GetLastDataCell](./getlastdatacell/) | 获取该行中的最后一个非空单元格。 |
| [ApplyStyle](./applystyle/) | 对整行应用格式。 |
| [Equals_Object](./equals_object/) | 检查此对象是否与另一个对象指向同一行。 |
| [Equals_Row](./equals_row/) | 检查此对象是否与另一个行对象指向同一行。 |
