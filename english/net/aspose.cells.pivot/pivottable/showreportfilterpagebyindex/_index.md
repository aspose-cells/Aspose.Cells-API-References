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
public void PivotTable_Method_ShowReportFilterPageByIndex()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46429_";
    Workbook wb = new Workbook(filePath + "a.xlsx");
    PivotTable pt = wb.Worksheets[1].PivotTables[0];
    pt.ShowReportFilterPage(pt.PageFields[0]);
    pt.ShowReportFilterPage(pt.PageFields[0]);
    pt.ShowReportFilterPage(pt.PageFields[0]);
    pt.ShowReportFilterPageByIndex(pt.PageFields[0].Position);
    pt.ShowReportFilterPageByName(pt.PageFields[0].Name);
    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
    Assert.AreEqual(wb.Worksheets.Count, 17);
    Assert.AreEqual(wb.Worksheets[15].Name.EndsWith("(5)"), true);
    Assert.AreEqual(wb.Worksheets[12].Name.EndsWith("(4)"), true);
    Assert.AreEqual(wb.Worksheets[9].Name.EndsWith("(3)"), true);
    Assert.AreEqual(wb.Worksheets[6].Name.EndsWith("(2)"), true);

    Assert.AreEqual("18", wb.Worksheets[1].Cells["A4"].StringValue);
    Assert.AreEqual("22", wb.Worksheets[2].Cells["A4"].StringValue);
    Assert.AreEqual("18", wb.Worksheets[3].Cells["A4"].StringValue);


}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


