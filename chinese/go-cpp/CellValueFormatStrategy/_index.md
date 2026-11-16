---
title: "CellValueFormatStrategy 枚举"
linktitle: "CellValueFormatStrategy"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CellValueFormatStrategy 枚举。封装在 Go 中表示 cellvalueformatstrategy 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

指定如何为单元格的值应用样式。

```go

type CellValueFormatStrategy int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [None](./none/) | 未格式化。 |
| [CellStyle](./cellstyle/) | 仅使用单元格的原始样式进行格式化。 |
| [DisplayStyle](./displaystyle/) | 使用单元格的显示样式进行格式化。 |
| [DisplayString](./displaystring/) | 获取在 MS Excel 中显示的字符串。与 <see cref="DisplayStyle"/> 的主要区别在于此选项还会考虑列宽的影响。如果列宽太小而无法完整显示格式化后的字符串，可能会显示 "#"，这与 MS Excel 的表现相同。 |
