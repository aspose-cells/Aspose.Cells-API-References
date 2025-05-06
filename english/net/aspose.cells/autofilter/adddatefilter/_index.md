---
title: AutoFilter.AddDateFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Adds a date filter
type: docs
url: /net/aspose.cells/autofilter/adddatefilter/
---
## AutoFilter.AddDateFilter method

Adds a date filter.

```csharp
public void AddDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dateTimeGroupingType | DateTimeGroupingType | The grouping type |
| year | Int32 | The year. |
| month | Int32 | The month. |
| day | Int32 | The day. |
| hour | Int32 | The hour. |
| minute | Int32 | The minute. |
| second | Int32 | The second. |

### Remarks

If DateTimeGroupingType is Year, only the param year effects. If DateTiemGroupingType is Month, only the param year and month effect.

### Examples

```csharp
// Called: worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);
public static void Method_Int32_()
        {
            // Creating a file stream containing the Excel file to be opened
            // Instantiating a Workbook object
            Workbook workbook = new Workbook(&quot;AutoFilterExampleTemplate.xlsx&quot;);
            // Accessing the first worksheet in the Excel file
            Worksheet worksheet = workbook.Worksheets[0];
            // Creating AutoFilter by giving the cells range of the heading row
            worksheet.AutoFilter.Range = &quot;A1:B8&quot;;
            // Filtering columns with specified values
            worksheet.AutoFilter.Filter(0, &quot;Bananas&quot;);
            worksheet.AutoFilter.Refresh();

            // Saving the modified Excel file.
            workbook.Save(&quot;AutoFilterExample.xlsx&quot;);
            workbook.Save(&quot;AutoFilterExample.pdf&quot;);

            // Instantiating a Workbook object
            workbook = new Workbook(&quot;AutoFilterExampleTemplate.xlsx&quot;);
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Additional code to demonstrate other functionalities of AutoFilter
            // Setting the range for AutoFilter
            worksheet.AutoFilter.Range = &quot;A1:B8&quot;;
            // Adding a filter
            worksheet.AutoFilter.AddFilter(0, &quot;Apples&quot;);
            // Adding a date filter
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save(&quot;AutoFilterExample2.xlsx&quot;);
            workbook.Save(&quot;AutoFilterExample2.pdf&quot;);

            // Instantiating a Workbook object
            workbook = new Workbook(&quot;AutoFilterExampleTemplate.xlsx&quot;);
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];
                        
            // Adding a font color filter
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save(&quot;AutoFilterExample3.xlsx&quot;);
            workbook.Save(&quot;AutoFilterExample3.pdf&quot;);

            // Instantiating a Workbook object
            workbook = new Workbook(&quot;AutoFilterExampleTemplate.xlsx&quot;);
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
            workbook.Save(&quot;AutoFilterExample4.xlsx&quot;);
            workbook.Save(&quot;AutoFilterExample4.pdf&quot;);

            // Instantiating a Workbook object
            workbook = new Workbook(&quot;AutoFilterExampleTemplate.xlsx&quot;);
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Matching blanks
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save(&quot;AutoFilterExample5.xlsx&quot;);
            workbook.Save(&quot;AutoFilterExample5.pdf&quot;);

            // Instantiating a Workbook object
            workbook = new Workbook(&quot;AutoFilterExampleTemplate.xlsx&quot;);
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Matching non-blanks
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save(&quot;AutoFilterExample6.xlsx&quot;);
            workbook.Save(&quot;AutoFilterExample6.pdf&quot;);

            // Instantiating a Workbook object
            workbook = new Workbook(&quot;AutoFilterExampleTemplate.xlsx&quot;);
            // Accessing the first worksheet in the Excel file
            worksheet = workbook.Worksheets[0];

            // Custom filter
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, &quot;Test&quot;);

            worksheet.AutoFilter.Refresh();
            // Saving the modified Excel file.
            workbook.Save(&quot;AutoFilterExample7.xlsx&quot;);
            workbook.Save(&quot;AutoFilterExample7.pdf&quot;);
        }
```

### See Also

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


