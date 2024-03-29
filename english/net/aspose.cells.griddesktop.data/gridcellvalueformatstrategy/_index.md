---
title: Enum GridCellValueFormatStrategy
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridDesktop.Data.GridCellValueFormatStrategy enum. Specifies how to apply style for the value of the cell
type: docs
url: /net/aspose.cells.griddesktop.data/gridcellvalueformatstrategy/
---
## GridCellValueFormatStrategy enumeration

Specifies how to apply style for the value of the cell.

```csharp
public enum GridCellValueFormatStrategy
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Not formatted. |
| CellStyle | `1` | Only formatted with the cell's original style. |
| DisplayStyle | `2` | Formatted with the cell's displayed style. |
| DisplayString | `3` | Gets the displayed string shown in ms excel. The main difference from DisplayStyle is this option also considers the effect of column width. If the column width is too small to show the formatted string completely, "#" may be shown, just like what ms excel does. |

### See Also

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


