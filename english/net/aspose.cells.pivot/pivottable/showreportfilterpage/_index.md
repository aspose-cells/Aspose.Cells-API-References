---
title: PivotTable.ShowReportFilterPage
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Show all the report filter pages according to PivotField the PivotField must be located in the PageFields
type: docs
url: /net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageField | PivotField | The PivotField object |

### Examples

```csharp
// Called: pt.ShowReportFilterPage(pt.PageFields[0]);
[Test]
        public void Method_PivotField_()
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

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


