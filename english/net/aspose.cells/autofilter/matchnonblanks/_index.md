---
title: AutoFilter.MatchNonBlanks
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Match all not blank cell in the list
type: docs
url: /net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Match all not blank cell in the list.

```csharp
public void MatchNonBlanks(int fieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |

### Examples

```csharp
// Called: worksheet.AutoFilter.MatchNonBlanks(0);
public static void AutoFilter_Method_MatchNonBlanks()
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
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


