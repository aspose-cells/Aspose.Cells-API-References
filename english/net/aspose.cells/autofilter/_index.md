---
title: Class AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AutoFilter class. Represents autofiltering for the specified worksheet
type: docs
url: /net/aspose.cells/autofilter/
---
## AutoFilter class

Represents autofiltering for the specified worksheet.

```csharp
public class AutoFilter
```

## Properties

| Name | Description |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Gets the collection of the filter columns. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Represents the range to which the specified AutoFilter applies. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Indicates whether the AutoFilter button for this column is visible. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Gets the data sorter. |

## Methods

| Name | Description |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Adds a date filter. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Adds a fill color filter. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Adds a filter for a filter column. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Adds a font color filter. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Adds an icon filter. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Filters a list with a custom criterion. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Filters a list with custom criteria. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Adds a dynamic filter. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Filters a list with specified criteria. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Filter the top 10 items in the list |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Gets the [`CellArea`](../cellarea/) where the this AutoFilter applies to. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Gets the [`CellArea`](../cellarea/) where the specified AutoFilter applies. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Match all blank cells in the list. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Match all not-blank cells in the list. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Refresh auto filters to hide or unhide the rows. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Gets all hidden rows' indexes. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Removes a date filter. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Remove the specific filter. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Removes a filter for a filter column. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Sets the range to which the specified AutoFilter applies. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Unhide all rows. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Creating a file stream containing the Excel file to be opened
            // Instantiating a Workbook object
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accessing the first worksheet in the Excel file
            Worksheet worksheet = workbook.Worksheets[0];
            // Creating AutoFilter by giving the cells range of the heading row
            worksheet.AutoFilter.Range = "A1:B8";
            // Filtering columns with specified values
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Saving the modified Excel file.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Instantiating a Workbook object
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Additional code to demonstrate other functionalities of AutoFilter
            // Setting the range for AutoFilter
            worksheet.AutoFilter.Range = "A1:B8";
            // Adding a filter
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Adding a date filter
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Instantiating a Workbook object
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];
                        
            // Adding a font color filter
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Instantiating a Workbook object
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Adding a fill color filter
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Instantiating a Workbook object
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Matching blanks
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Instantiating a Workbook object
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Matching non-blanks
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Instantiating a Workbook object
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Custom filter
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


