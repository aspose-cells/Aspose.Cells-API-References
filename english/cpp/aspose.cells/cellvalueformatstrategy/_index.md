---
title: Aspose::Cells::CellValueFormatStrategy enum
linktitle: CellValueFormatStrategy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CellValueFormatStrategy enum. Specifies how to apply style for the value of the cell in C++.'
type: docs
weight: 18000
url: /cpp/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enum


Specifies how to apply style for the value of the cell.

```cpp
enum class CellValueFormatStrategy
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | 0 | Not formatted. |
| CellStyle | 1 | Only formatted with the cell's original style. |
| DisplayStyle | 2 | Formatted with the cell's displayed style. |
| DisplayString | 3 | Gets the displayed string shown in ms excel. The main difference from [DisplayStyle](./) is this option also considers the effect of column width. If the column width is too small to show the formatted string completely, "#" may be shown, just like what ms excel does. |

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
