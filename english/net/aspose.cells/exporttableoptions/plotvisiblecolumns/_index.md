---
title: ExportTableOptions.PlotVisibleColumns
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Only exports visible columns
type: docs
url: /net/aspose.cells/exporttableoptions/plotvisiblecolumns/
---
## ExportTableOptions.PlotVisibleColumns property

Only exports visible columns.

```csharp
public bool PlotVisibleColumns { get; set; }
```

### Examples

```csharp
// Called: options.PlotVisibleColumns = true;
[Test]
        public void Property_PlotVisibleColumns()
        {
            var book = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;43935.xlsx&quot;);
            var manpowerdevt = book.Worksheets[0];

            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.PlotVisibleColumns = true;

            DataTable dataTable = new DataTable();
            dataTable = manpowerdevt.Cells.ExportDataTable(0, 0, manpowerdevt.Cells.MaxRow + 1, manpowerdevt.Cells.MaxColumn + 1, options);
            Assert.AreEqual(4, dataTable.Columns.Count);
        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


