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
[Test]
        public void Type_ColorFilter()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/FilterTest.xlsx&quot;);
            AutoFilter filter = workbook.Worksheets[0].AutoFilter;
            Cells cells = workbook.Worksheets[0].Cells;
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            filter.AddFontColorFilter(1,cr);
            filter.Refresh();
            Assert.IsTrue(cells.IsRowHidden(1));
            Assert.IsTrue(cells.IsRowHidden(2));
            Assert.IsTrue(cells.IsRowHidden(3));
            Assert.IsFalse(cells.IsRowHidden(4));
            //workbook.Save(Constants.destPath + &quot;TestFontColorFilter01.xlsx&quot;);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);// new Workbook(Constants.destPath + &quot;TestFontColorFilter01.xlsx&quot;);

            filter = workbook.Worksheets[0].AutoFilter;
            FilterColumn fc = filter.FilterColumns[1];
            Assert.AreEqual(FilterType.ColorFilter, fc.FilterType);
            
            ColorFilter cf = fc.Filter as ColorFilter;
            Assert.IsFalse(cf.FilterByFillColor);
            AssertHelper.AreEqual(cf.GetColor(workbook.Worksheets), Color.Red);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


