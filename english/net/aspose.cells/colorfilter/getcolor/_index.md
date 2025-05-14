---
title: ColorFilter.GetColor
second_title: Aspose.Cells for .NET API Reference
description: ColorFilter method. Gets the color of this filter
type: docs
url: /net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Gets the color of this filter.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheets | WorksheetCollection |  |

### Examples

```csharp
// Called: AssertHelper.AreEqual(cf.GetColor(workbook.Worksheets), Color.Red);
public void ColorFilter_Method_GetColor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/FilterTest.xlsx");
    AutoFilter filter = workbook.Worksheets[0].AutoFilter;
    Cells cells = workbook.Worksheets[0].Cells;
    CellsColor cr =  workbook.CreateCellsColor();
    cr.Color = Color.Red;
    filter.AddFillColorFilter(3, BackgroundType.Solid, cr, cr);
    filter.Refresh();
    Assert.IsTrue(cells.IsRowHidden(1));
    Assert.IsTrue(cells.IsRowHidden(2));
    Assert.IsTrue(cells.IsRowHidden(3));
    Assert.IsFalse(cells.IsRowHidden(4));
    //workbook.Save(Constants.destPath + "example.xlsx");
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);// new Workbook(Constants.destPath + "example.xlsx");

    filter = workbook.Worksheets[0].AutoFilter;
    FilterColumn fc = filter.FilterColumns[3];
    Assert.AreEqual(FilterType.ColorFilter, fc.FilterType);
    ColorFilter cf = fc.Filter as ColorFilter;

    Assert.IsTrue(cf.FilterByFillColor);
    AssertHelper.AreEqual(cf.GetColor(workbook.Worksheets), Color.Red);
}
```

### See Also

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


