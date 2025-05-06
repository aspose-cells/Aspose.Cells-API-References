---
title: AutoFilter.RemoveFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Removes a filter for a filter column
type: docs
url: /net/aspose.cells/autofilter/removefilter/
---
## RemoveFilter(int, string) {#removefilter_1}

Removes a filter for a filter column.

```csharp
public void RemoveFilter(int fieldIndex, string criteria)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). It only can be null or be one of the cells' value in this column. |

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveFilter(int) {#removefilter}

Remove the specific filter.

```csharp
public void RemoveFilter(int fieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The specific filter index |

### Examples

```csharp
// Called: filter.RemoveFilter(1);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;AutoFilter/N54305.xlsx&quot;);
            Worksheet worksheet = wb.Worksheets[0];

            Style style = worksheet.Cells[&quot;A14&quot;].GetDisplayStyle();
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
                &quot;ColorFilter.GetColor() for font color filter&quot;);

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
                &quot;ColorFilter.GetColor() for fill color filter&quot;);

            worksheet = wb.Worksheets[1];
            filter = worksheet.AutoFilter;

            // filter Sheet2.B3 Cell fill color success
            style = worksheet.Cells[&quot;B3&quot;].GetDisplayStyle();
            foregroundColor.Color = style.ForegroundColor;
            backgroundColor.Color = style.BackgroundColor;
            filter.AddFillColorFilter(1, style.Pattern, foregroundColor, backgroundColor);
            filter.Refresh(true);
            CheckVisibleRows(new int[] { 0, 2, 5, 7, }, worksheet.Cells);

            filter.RemoveFilter(1);
            // filter Sheet2.A4 Cell fill color fail
            style = worksheet.Cells[&quot;A4&quot;].GetDisplayStyle();
            foregroundColor.Color = style.ForegroundColor;
            backgroundColor.Color = style.BackgroundColor;
            filter.AddFillColorFilter(0, style.Pattern, foregroundColor, backgroundColor);
            filter.Refresh(true);
            CheckVisibleRows(new int[] { 0, 3, 4, 7, }, worksheet.Cells);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


