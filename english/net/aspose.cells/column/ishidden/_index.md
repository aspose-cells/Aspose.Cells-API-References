---
title: Column.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: Column property. Indicates whether the column is hidden
type: docs
url: /net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Indicates whether the column is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue( column.IsHidden);
[Test]
        public void Property_IsHidden()
        {
            var wb = new Workbook(Constants.sourcePath + "CellsNet54793.xlsx");
            var ws = wb.Worksheets[0];
            var column = ws.Cells.Columns[1];

            // True
            Assert.IsTrue(column.IsHidden);

            ws.AutoFitColumns(new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            });

            // False
           Assert.IsTrue( column.IsHidden);
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


