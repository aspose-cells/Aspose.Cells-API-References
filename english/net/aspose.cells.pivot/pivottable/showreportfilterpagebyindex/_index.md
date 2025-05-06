---
title: PivotTable.ShowReportFilterPageByIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Show all the report filter pages according to the position index in the PageFields
type: docs
url: /net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

Show all the report filter pages according to the position index in the PageFields

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| posIndex | Int32 | The position index in the PageFields |

### Examples

```csharp
// Called: pt.ShowReportFilterPageByIndex(pt.PageFields[0].Position);
[Test]
        public void Method_Int32_()
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

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


