---
title: ExportTableOptions.RenameStrategy
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Strategy for duplicate names of columns
type: docs
url: /net/aspose.cells/exporttableoptions/renamestrategy/
---
## ExportTableOptions.RenameStrategy property

Strategy for duplicate names of columns.

```csharp
public RenameStrategy RenameStrategy { get; set; }
```

### Examples

```csharp
// Called: options.RenameStrategy = RenameStrategy.Letter;
[Test]
        public void Property_RenameStrategy()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + @&quot;CellsNet44416.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            ExportTableOptions options = new ExportTableOptions();
            options.RenameStrategy = RenameStrategy.Letter;
            options.ExportColumnName = true;
            DataTable dt = cells.ExportDataTable(0, 0, 3, 6, options);
           Assert.AreEqual(dt.Columns[3].ColumnName,&quot;bA&quot;);
        }
```

### See Also

* enum [RenameStrategy](../../renamestrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


