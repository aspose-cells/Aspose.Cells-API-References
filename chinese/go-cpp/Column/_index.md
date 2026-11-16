---
title: "Column 类"
linktitle: "列"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Column 类。封装在 Go 中表示列的对象。"
type: docs
weight: 200
url: /zh/go-cpp/column/
---

## Column class

表示工作表中的单列。

```go

type Column struct  {
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
| [GetIndex](./getindex/) | 获取此列的索引。 |
| [GetWidth](./getwidth/) | 获取和设置列宽，单位为字符。 |
| [SetWidth](./setwidth/) | 获取和设置列宽，单位为字符。 |
| [GetGroupLevel](./getgrouplevel/) | 获取列的分组级别。 |
| [SetGroupLevel](./setgrouplevel/) | 获取列的分组级别。 |
| [IsHidden](./ishidden/) | 指示列是否隐藏。 |
| [SetIsHidden](./setishidden/) | 指示列是否隐藏。 |
| [GetHasCustomStyle](./gethascustomstyle/) | 指示此列是否具有自定义样式设置（不同于从工作簿继承的默认样式）。 |
| [ApplyStyle](./applystyle/) | 对整列应用格式。 |
| [GetStyle](./getstyle/) | 获取此列的样式。 |
| [SetStyle](./setstyle/) | 设置此列的样式。 |
| [IsCollapsed](./iscollapsed/) | 列是否折叠 |
| [SetIsCollapsed](./setiscollapsed/) | 列是否折叠 |
