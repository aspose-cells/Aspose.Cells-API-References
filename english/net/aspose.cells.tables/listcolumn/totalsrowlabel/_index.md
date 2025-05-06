---
title: ListColumn.TotalsRowLabel
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the display labels of total row
type: docs
url: /net/aspose.cells.tables/listcolumn/totalsrowlabel/
---
## ListColumn.TotalsRowLabel property

Gets and sets the display labels of total row.

```csharp
public string TotalsRowLabel { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;88&amp;quot;, table.ListColumns[0].TotalsRowLabel);
[Test]
        public void Property_TotalsRowLabel()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET53284.xlsx&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            ListObject table = wb.Worksheets[0].ListObjects[0];
            table.PutCellValue(4, 0, &quot;88&quot;);
            table.PutCellValue(4, 1, 88);
            table.PutCellFormula(4, 2, &quot;=C3&quot;);
            Assert.AreEqual(&quot;88&quot;, table.ListColumns[0].TotalsRowLabel);

            wb.Save(Constants.destPath + &quot;CELLSNET53284.xlsx&quot;);
        }
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


