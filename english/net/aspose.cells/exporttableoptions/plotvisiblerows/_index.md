---
title: ExportTableOptions.PlotVisibleRows
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Only exports visible rows
type: docs
url: /net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Only exports visible rows.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Examples

```csharp
// Called: PlotVisibleRows = true
[Test]
        public void Property_PlotVisibleRows()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46667.xlsx&quot;);

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Specify export table options
            ExportTableOptions exportOptions = new ExportTableOptions()
            {
                PlotVisibleCells = true,
                PlotVisibleColumns = true,
                PlotVisibleRows = true
            };

            // Export the data from worksheet with export options
            DataTable dataTable = worksheet.Cells.ExportDataTable(1, 0, 5, 7, exportOptions);
            Assert.AreEqual(1, dataTable.Rows.Count);

        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


