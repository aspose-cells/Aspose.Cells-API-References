---
title: Cells.ImportDataView
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports a DataView into a worksheet
type: docs
url: /net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Imports a DataView into a worksheet.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | The DataView object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |

### Return Value

Total number of rows imported

### Examples

```csharp
// Called: cells.ImportDataView(dataview, 1048576, 0);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = &quot;testImportDataView_Exception_003&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataView dataview = getDataView();
            cells.ImportDataView(dataview, 1048576, 0);
            string msg = message + &quot;cells.ImportDataView(dataview, 1048576, 0)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


