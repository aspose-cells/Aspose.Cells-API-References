---
title: Cells.ExportArray
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Exports data in the Cells collection to a twodimension array object
type: docs
url: /net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Exports data in the [`Cells`](../) collection to a two-dimension array object.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be exported |
| totalColumns | Int32 | Number of columns to be exported |

### Return Value

Exported cell value array object.

### Examples

```csharp
// Called: cells.ExportArray(0, 0, 2, 16385);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = "testExportArray_Exception_009";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.ExportArray(0, 0, 2, 16385);
            string msg = message + "cells.ExportArray(2, 2, 1048576, 16384)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


