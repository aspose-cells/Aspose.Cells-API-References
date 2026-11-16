---
title: "PdfBookmarkEntry 类"
linktitle: "PdfBookmarkEntry"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PdfBookmarkEntry 类。封装了在 Go 中表示 pdfbookmarkentry 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry 是 PDF 书签中的一个条目。如果当前实例的 Text 属性为 null 或 \"\"，则当前实例将被隐藏，子项将插入到当前层级。

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetText](./gettext/) | 书签的标题。 |
| [SetText](./settext/) | 书签的标题。 |
| [GetDestination](./getdestination/) | 书签链接指向的单元格。 |
| [SetDestination](./setdestination/) | 书签链接指向的单元格。 |
| [GetDestinationName](./getdestinationname/) | 获取或设置目标的名称。 |
| [SetDestinationName](./setdestinationname/) | 获取或设置目标的名称。 |
| [IsOpen](./isopen/) | 当此属性为 true 时，bookmarkentry 将展开，否则将折叠。 |
| [SetIsOpen](./setisopen/) | 当此属性为 true 时，bookmarkentry 将展开，否则将折叠。 |
| [IsCollapse](./iscollapse/) | 当此属性为 true 时，bookmarkentry 将折叠，否则将展开。 |
| [SetIsCollapse](./setiscollapse/) | 当此属性为 true 时，bookmarkentry 将折叠，否则将展开。 |
