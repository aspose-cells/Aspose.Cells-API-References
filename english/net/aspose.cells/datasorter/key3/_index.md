---
title: DataSorter.Key3
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents third sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Key3 { get; set; }
```

### Examples

```csharp
// Called: wb.DataSorter.Key3 = wb.Worksheets[0].Cells[&amp;quot;C2&amp;quot;].Column;
[Test]
        public void Property_Key3()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Sort/CellsNet45421.xls&quot;);
            wb.CalculateFormula();

            wb.DataSorter.Order1 = SortOrder.Ascending;
            wb.DataSorter.Key1 = wb.Worksheets[0].Cells[&quot;D2&quot;].Column;

            wb.DataSorter.Order2 = SortOrder.Ascending;
            wb.DataSorter.Key2 = wb.Worksheets[0].Cells[&quot;E2&quot;].Column;

            wb.DataSorter.Order3 = SortOrder.Ascending;
            wb.DataSorter.Key3 = wb.Worksheets[0].Cells[&quot;C2&quot;].Column;

            CellArea ca = new CellArea();
            ca.StartRow = 1;
            ca.StartColumn = 0;
            ca.EndRow = 10;
            ca.EndColumn = 9;

            wb.DataSorter.Sort(wb.Worksheets[0].Cells, ca);
            Assert.AreEqual(&quot;=F2/D2*7&quot;, wb.Worksheets[0].Cells[&quot;G2&quot;].Formula);
            Assert.AreEqual(&quot;=F3/D3*7&quot;, wb.Worksheets[0].Cells[&quot;G3&quot;].Formula);
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


