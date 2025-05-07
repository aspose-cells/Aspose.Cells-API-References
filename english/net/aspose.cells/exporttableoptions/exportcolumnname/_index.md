---
title: ExportTableOptions.ExportColumnName
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false
type: docs
url: /net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Indicates whether the data in the first row are exported to the column name of the DataTable. The default value is false.

```csharp
public bool ExportColumnName { get; set; }
```

### Examples

```csharp
// Called: options.ExportColumnName = true;
[Test]
        public void Property_ExportColumnName()
        {
            var book = new Aspose.Cells.Workbook(Constants.sourcePath + "43935.xlsx");
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


