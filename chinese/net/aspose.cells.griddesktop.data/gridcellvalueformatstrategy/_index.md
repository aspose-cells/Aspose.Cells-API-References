---
title: "枚举 GridCellValueFormatStrategy"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridDesktop.Data.GridCellValueFormatStrategy 枚举。指定如何为单元格的值应用样式"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridcellvalueformatstrategy/
---
## GridCellValueFormatStrategy enumeration

指定如何为单元格的值应用样式。

```csharp
public enum GridCellValueFormatStrategy
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 未格式化。 |
| CellStyle | `1` | 仅使用单元格的原始样式进行格式化。 |
| DisplayStyle | `2` | 使用单元格的显示样式进行格式化。 |
| DisplayString | `3` | 获取在 ms excel 中显示的字符串。与 DisplayStyle 的主要区别在于此选项还会考虑列宽的影响。如果列宽过小而无法完整显示格式化后的字符串，可能会显示 "#"，就像 ms excel 的表现一样。 |

### 另请参见

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


