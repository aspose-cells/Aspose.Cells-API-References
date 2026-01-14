---
title: FilterColumn.ColorFilter
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets ColorFilter for filtering data by color
type: docs
url: /net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Gets [`ColorFilter`](../../colorfilter/) for filtering data by color.

```csharp
public ColorFilter ColorFilter { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add sample data with colors
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Apply auto filter
                worksheet.AutoFilter.Range = "A1:A4";

                // Get the filter column
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Access the ColorFilter property (read-only)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // Display ColorFilter properties
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Save the workbook
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


