---
title: Cells.LastCell
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the last cell in this worksheet
type: docs
url: /net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Gets the last cell in this worksheet.

```csharp
public Cell LastCell { get; }
```

### Remarks

Returns null if there is no data in the worksheet.

### Examples

```csharp
// Called: for (int row = 1; row &amp;lt;= sheet.Cells.LastCell.Row; row++)
[Test]
        public void Property_LastCell()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet56029.xlsx&quot;);


            //Replace &quot;Person1&quot; by &quot;Person one&quot;:
            Worksheet sheet = wb.Worksheets[0];
            for (int row = 1; row &lt;= sheet.Cells.LastCell.Row; row++)
            {
                if (sheet.Cells[row, 0].Value.ToString() == &quot;Person1&quot;)
                {
                    sheet.Cells[row, 0].Value = &quot;Person one&quot;;
                }
            }


            wb.Worksheets[1].PivotTables[0].RefreshData();
            wb.Worksheets[1].PivotTables[0].CalculateData();
            //  wb.Worksheets.RefreshAll();
            Assert.AreEqual(&quot;Person2&quot;, wb.Worksheets[1].Cells[&quot;A8&quot;].StringValue);
            Assert.AreEqual(&quot;Person one&quot;, wb.Worksheets[1].Cells[&quot;A18&quot;].StringValue);

        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


