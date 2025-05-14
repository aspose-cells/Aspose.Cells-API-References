---
title: Class ColorFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ColorFilter class. Represents filtering the range by color
type: docs
url: /net/aspose.cells/colorfilter/
---
## ColorFilter class

Represents filtering the range by color.

```csharp
public class ColorFilter
```

## Properties

| Name | Description |
| --- | --- |
| [FilterByFillColor](../../aspose.cells/colorfilter/filterbyfillcolor/) { get; set; } | Whether filter by the cell's fill color. |

## Methods

| Name | Description |
| --- | --- |
| [GetColor](../../aspose.cells/colorfilter/getcolor/)(WorksheetCollection) | Gets the color of this filter. |

### Examples

```csharp
// Called: ColorFilter cf = fc.Filter as ColorFilter;
public void Cells_Type_ColorFilter()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


