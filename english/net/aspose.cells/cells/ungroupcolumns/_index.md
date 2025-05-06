---
title: Cells.UngroupColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Ungroups columns
type: docs
url: /net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Ungroups columns.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be ungrouped. |
| lastIndex | Int32 | The last column index to be ungrouped. |

### Examples

```csharp
// Called: worksheet.Cells.UngroupColumns(0, 2);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            WorksheetCollection sheets = wb.Worksheets;

            Worksheet worksheet = sheets[0];

            // Ungrouping first six rows (from 0 to 5)
            worksheet.Cells.UngroupRows(0, 5);

            // Ungrouping first three columns (from 0 to 2)
            worksheet.Cells.UngroupColumns(0, 2);
            wb.Save(Constants.destPath + &quot;CELLSNET58144.xls&quot;);

        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


