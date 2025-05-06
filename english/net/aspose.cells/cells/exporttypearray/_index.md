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
// Called: CellValueType[,] arr = cells.ExportTypeArray(1, 1, 1048576, 16384);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = &quot;testExportTypeArray_Exception_009&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            CellValueType[,] arr = cells.ExportTypeArray(1, 1, 1048576, 16384);
            string msg = message + &quot;cells.ExportTypeArray(1, 1, 1048576, 16384)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


