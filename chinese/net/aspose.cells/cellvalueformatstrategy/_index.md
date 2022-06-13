---
title: CellValueFormatStrategy
second_title: Aspose.Cells for .NET API 参考
description: 指定如何为单元格的值应用样式
type: docs
weight: 260
url: /zh/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

指定如何为单元格的值应用样式。

```csharp
public enum CellValueFormatStrategy
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| None | `0` | 未格式化。 |
| CellStyle | `1` | 仅使用单元格的原始样式格式化。 |
| DisplayStyle | `2` | 以单元格的显示样式格式化。 |
| DisplayString | `3` | 获取 ms excel 中显示的字符串。 与DisplayStyle的主要区别在于该选项还考虑了列宽的影响。 如果列宽太小而无法完整显示格式化字符串，可能会显示 "#"，就像 ms excel 所做的那样。 |

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->