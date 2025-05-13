---
title: Cells.UnMerge
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Unmerges a specified range of merged cells
type: docs
url: /net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Unmerges a specified range of merged cells.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |

### Examples

```csharp
// Called: cells.UnMerge(0, 16384, 2, 2);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Cells_Method_UnMerge()
        {
            caseName = "testUnMerge_Exception_006";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.UnMerge(0, 16384, 2, 2);
            string msg = message + "cells.UnMerge(0, 16384, 2, 2)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


