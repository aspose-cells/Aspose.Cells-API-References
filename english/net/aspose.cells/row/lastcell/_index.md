---
title: Row.LastCell
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the last cell object in the row
type: docs
url: /net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Gets the last cell object in the row.

```csharp
public Cell LastCell { get; }
```

### Examples

```csharp
// Called: object v = row.LastCell.Value;
[Test]
        public void Property_LastCell()
        {
            TxtLoadOptions opts = new TxtLoadOptions(LoadFormat.Csv);
            Workbook wb = new Workbook(Constants.TemplatePath + &quot;Test_151622.csv&quot;, opts);
            Worksheet ws = wb.Worksheets[wb.Worksheets.ActiveSheetIndex];
            Row row = ws.Cells.Rows[0];
            object v = row.LastCell.Value;
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


