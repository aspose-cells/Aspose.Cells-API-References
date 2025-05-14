---
title: Enum FilterType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FilterType enum. The filter type
type: docs
url: /net/aspose.cells/filtertype/
---
## FilterType enumeration

The filter type.

```csharp
public enum FilterType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| ColorFilter | `0` | Filter by fill color of the cell. |
| CustomFilters | `1` | Custom filter type. |
| DynamicFilter | `2` | Dynamic filter type. |
| MultipleFilters | `3` | When multiple values are chosen to filter by, or when a group of date values are chosen to filter by, this element groups those criteria together. |
| IconFilter | `4` | Filter by icon of conditional formatting. |
| Top10 | `5` | Top 10 filter. |
| None | `6` | No filter. |

### Examples

```csharp
// Called: Assert.AreEqual(FilterType.ColorFilter, fc.FilterType);
public void Cells_Type_FilterType()
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


