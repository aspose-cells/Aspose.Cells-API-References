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
public void PivotTable_Method_ShowReportFilterPage()
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

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


