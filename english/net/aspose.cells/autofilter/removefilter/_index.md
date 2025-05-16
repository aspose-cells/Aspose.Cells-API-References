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

### Examples

```csharp
namespace AsposeCellsExamples.AutoFilterMethodRemoveFilterWithInt32StringDemo
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodRemoveFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Create a new workbook and access the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data for demonstration
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["C2"].PutValue(999.99);
            
            worksheet.Cells["A3"].PutValue("Novel");
            worksheet.Cells["B3"].PutValue("Books");
            worksheet.Cells["C3"].PutValue(19.99);
            
            worksheet.Cells["A4"].PutValue("Smartphone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["C4"].PutValue(599.99);

            // Set auto filter range (headers + 3 data rows)
            worksheet.AutoFilter.Range = "A1:C4";

            try
            {
                AutoFilter autoFilter = worksheet.AutoFilter;
                
                // Apply filter on Category column (fieldIndex 1) for "Electronics"
                autoFilter.AddFilter(1, "Electronics");
                autoFilter.Refresh(); // Apply filter to hide non-matching rows

                // Remove the specific filter from Category column
                autoFilter.RemoveFilter(1, "Electronics");
                autoFilter.Refresh(); // Re-apply filter (now shows all rows)

                Console.WriteLine("RemoveFilter executed: Electronics filter removed from Category column.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("RemoveFilterDemo.xlsx");
        }
    }
}
```

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
public void AutoFilter_Method_RemoveFilter()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
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

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


