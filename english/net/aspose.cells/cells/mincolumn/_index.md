---
title: Cells.MinColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum column index of those cells that have been instantiated in the collectiondoes not include the column where style is defined for the whole column but no cell has been instantiated in it
type: docs
url: /net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

```csharp
public int MinColumn { get; }
```

### Examples

```csharp
// Called: cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);
[Test]
        public void Property_MinColumn()
        {
            string path = Constants.sourcePath + &quot;Charts/&quot;;
            var workbook = new Workbook(path + &quot;CELLSNET49179.xlsx&quot;);
            var ws = workbook.Worksheets[1];
            Cells cells = ws.Cells;
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);
            workbook.Save(Constants.destPath + &quot;CELLSNET49179_out.xlsx&quot;);
            var newWorkbook = new Workbook(Constants.destPath + &quot;CELLSNET49179_out.xlsx&quot;); // reopen the saved xlsx
            newWorkbook.Worksheets[1].Cells[&quot;E4&quot;].PutValue(&quot;CELLSNET49179&quot;); // apply the text to the referenced cell
            //newWorkbook.Worksheets[1].Cells[&quot;C4&quot;].PutValue(&quot;test2&quot;);
            //newWorkbook.Save(path + &quot;out.xlsx&quot;); // axis title missing
            Aspose.Cells.Charts.Chart chart1 = newWorkbook.Worksheets[0].Charts[0];
            string _linkedSource = chart1.ValueAxis.Title.LinkedSource;
            Assert.AreEqual(&quot;=Sheet1!$E$4&quot;, _linkedSource);
            string _title = chart1.ValueAxis.Title.Text;
            Assert.AreEqual(&quot;CELLSNET49179&quot;, _title);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


