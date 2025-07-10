﻿---
title: Aspose::Cells::Cells::GetCellStyle method
linktitle: GetCellStyle
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Cells::GetCellStyle method. Get the style of given cell in C++.'
type: docs
weight: 14400
url: /cpp/aspose.cells/cells/getcellstyle/
---
## Cells::GetCellStyle method


Get the style of given cell.

```cpp
Style Aspose::Cells::Cells::GetCellStyle(int32_t row, int32_t column)
```


| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | row index |
| column | int32_t | column |

## ReturnValue

the style of given cell.
## Remarks



The returned style is only the one set for the cell or inherited from the row/column of the cell, does not include the applied properties by other settings such as conditional formattings.
## See Also

* Class [Style](../../style/)
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
