---
title: Cells.ImportDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports a DataRow into the Excel file
type: docs
url: /net/aspose.cells/cells/importdatarow/
---
## Cells.ImportDataRow method

Imports a DataRow into the Excel file.

```csharp
public void ImportDataRow(DataRow dataRow, int row, int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataRow | DataRow | DataRow object. |
| row | Int32 | Row index. |
| firstColumn | Int32 | First column index. |

### Examples

```csharp
// Called: cells.ImportDataRow(datatable.Rows[0], 1048576, 0);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = &quot;testImportDataRow_Exception_003&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = getDataTable();
            cells.ImportDataRow(datatable.Rows[0], 1048576, 0);
            string msg = message + &quot;cells.ImportDataRow(datatable.Rows[0], 1048576, 0)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


