---
title: Cells.ExportTypeArray
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Exports cell value type in the Cells collection to a twodimension array object
type: docs
url: /net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

Exports cell value type in the [`Cells`](../) collection to a two-dimension array object.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be exported. |
| totalColumns | Int32 | Number of columns to be exported. |

### Return Value

Exported array object representing cell value types.

### Examples

```csharp
// Called: CellValueType[,] arr = cells.ExportTypeArray(-1, 0, 2, 2);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Cells_Method_ExportTypeArray()
        {
            caseName = "testExportTypeArray_Exception_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            CellValueType[,] arr = cells.ExportTypeArray(-1, 0, 2, 2);
            string msg = message + "cells.ExportTypeArray(-1, 0, 2, 2)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


