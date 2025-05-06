---
title: AutoFilter.AddFillColorFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Adds a fill color filter
type: docs
url: /net/aspose.cells/autofilter/addfillcolorfilter/
---
## AutoFilter.AddFillColorFilter method

Adds a fill color filter.

```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor, 
    CellsColor backgroundColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| pattern | BackgroundType | The background pattern type. |
| foregroundColor | CellsColor | The foreground color. |
| backgroundColor | CellsColor | The background color. |

### Examples

```csharp
// Called: filter.AddFillColorFilter(3, BackgroundType.Solid, cr, cr);
[Test]
        public void Method_CellsColor_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/FilterTest.xlsx&quot;);
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
            //workbook.Save(Constants.destPath + &quot;TestColorFilter01.xlsx&quot;);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);// new Workbook(Constants.destPath + &quot;TestColorFilter01.xlsx&quot;);

            filter = workbook.Worksheets[0].AutoFilter;
            FilterColumn fc = filter.FilterColumns[3];
            Assert.AreEqual(FilterType.ColorFilter, fc.FilterType);
            ColorFilter cf = fc.Filter as ColorFilter;

            Assert.IsTrue(cf.FilterByFillColor);
            AssertHelper.AreEqual(cf.GetColor(workbook.Worksheets), Color.Red);
        }
```

### See Also

* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


