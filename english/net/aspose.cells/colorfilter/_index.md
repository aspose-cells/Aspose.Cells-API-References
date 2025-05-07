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
// Called: ((ColorFilter)filter.FilterColumns[0].Filter).GetColor(wb.Worksheets),
[Test]
        public void Type_ColorFilter()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "AutoFilter/N54305.xlsx");
            Worksheet worksheet = wb.Worksheets[0];

            Style style = worksheet.Cells["A14"].GetDisplayStyle();
            CellsColor cellColor = wb.CreateCellsColor();
            cellColor.Color = style.Font.Color;

            // filter Sheet1.A14 Cell font color fail
            AutoFilter filter = worksheet.AutoFilter;
            filter.AddFontColorFilter(0, cellColor);
            filter.Refresh(true);
            int[] visibleRows = new int[] { 0, 12, 13, 14, 15, 18, 19, 20, 21, 33, 36, 37};
            CheckVisibleRows(visibleRows, worksheet.Cells);
            AssertHelper.AreEqual(cellColor.Color,
                ((ColorFilter)filter.FilterColumns[0].Filter).GetColor(wb.Worksheets),
                "ColorFilter.GetColor() for font color filter");

            // filter Sheet1.A14 Cell fill color fail
            CellsColor foregroundColor = wb.CreateCellsColor();
            CellsColor backgroundColor = wb.CreateCellsColor();
            foregroundColor.Color = style.ForegroundColor;
            backgroundColor.Color = style.BackgroundColor;
            filter.AddFillColorFilter(0, style.Pattern, foregroundColor, backgroundColor);
            filter.Refresh(true);
            CheckVisibleRows(visibleRows, worksheet.Cells);
            AssertHelper.AreEqual(foregroundColor.Color,
                ((ColorFilter)filter.FilterColumns[0].Filter).GetColor(wb.Worksheets),
                "ColorFilter.GetColor() for fill color filter");

            worksheet = wb.Worksheets[1];
            filter = worksheet.AutoFilter;

            // filter Sheet2.B3 Cell fill color success
            style = worksheet.Cells["B3"].GetDisplayStyle();
            foregroundColor.Color = style.ForegroundColor;
            backgroundColor.Color = style.BackgroundColor;
            filter.AddFillColorFilter(1, style.Pattern, foregroundColor, backgroundColor);
            filter.Refresh(true);
            CheckVisibleRows(new int[] { 0, 2, 5, 7, }, worksheet.Cells);

            filter.RemoveFilter(1);
            // filter Sheet2.A4 Cell fill color fail
            style = worksheet.Cells["A4"].GetDisplayStyle();
            foregroundColor.Color = style.ForegroundColor;
            backgroundColor.Color = style.BackgroundColor;
            filter.AddFillColorFilter(0, style.Pattern, foregroundColor, backgroundColor);
            filter.Refresh(true);
            CheckVisibleRows(new int[] { 0, 3, 4, 7, }, worksheet.Cells);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


