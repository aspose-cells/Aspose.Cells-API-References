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
public void PivotField_Property_Position()
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

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


