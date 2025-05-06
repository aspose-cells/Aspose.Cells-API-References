---
title: PivotField.Position
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the index of PivotField in the region
type: docs
url: /net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Represents the index of [`PivotField`](../) in the region.

```csharp
public int Position { get; }
```

### Examples

```csharp
// Called: pt.ShowReportFilterPageByIndex(pt.PageFields[0].Position);
[Test]
        public void Property_Position()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46429_&quot;;
            Workbook wb = new Workbook(filePath + &quot;a.xlsx&quot;);
            PivotTable pt = wb.Worksheets[1].PivotTables[0];
            pt.ShowReportFilterPage(pt.PageFields[0]);
            pt.ShowReportFilterPage(pt.PageFields[0]);
            pt.ShowReportFilterPage(pt.PageFields[0]);
            pt.ShowReportFilterPageByIndex(pt.PageFields[0].Position);
            pt.ShowReportFilterPageByName(pt.PageFields[0].Name);
            wb.Save(Constants.PivotTableDestPath + &quot;NET46429.xlsx&quot;);
            Assert.AreEqual(wb.Worksheets.Count, 17);
            Assert.AreEqual(wb.Worksheets[15].Name.EndsWith(&quot;(5)&quot;), true);
            Assert.AreEqual(wb.Worksheets[12].Name.EndsWith(&quot;(4)&quot;), true);
            Assert.AreEqual(wb.Worksheets[9].Name.EndsWith(&quot;(3)&quot;), true);
            Assert.AreEqual(wb.Worksheets[6].Name.EndsWith(&quot;(2)&quot;), true);

            Assert.AreEqual(&quot;18&quot;, wb.Worksheets[1].Cells[&quot;A4&quot;].StringValue);
            Assert.AreEqual(&quot;22&quot;, wb.Worksheets[2].Cells[&quot;A4&quot;].StringValue);
            Assert.AreEqual(&quot;18&quot;, wb.Worksheets[3].Cells[&quot;A4&quot;].StringValue);


        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


