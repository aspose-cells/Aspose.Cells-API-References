---
title: ColorFilter.FilterByFillColor
second_title: Aspose.Cells for .NET API Reference
description: ColorFilter property. Whether filter by the cells fill color
type: docs
url: /net/aspose.cells/colorfilter/filterbyfillcolor/
---
## ColorFilter.FilterByFillColor property

Whether filter by the cell's fill color.

```csharp
public bool FilterByFillColor { get; set; }
```

### Remarks

True: cell's fill color; False: cell's font color.

### Examples

```csharp
// Called: Assert.IsTrue(cf.FilterByFillColor);
[Test]
        public void Property_FilterByFillColor()
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

* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


