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
// Called: cells.ImportDataRow(datatable.Rows[0], -1, 0);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = "testImportDataRow_Exception_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = getDataTable();
            cells.ImportDataRow(datatable.Rows[0], -1, 0);
            string msg = message + "cells.ImportDataRow(datatable.Rows[0], -1, 0)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


