---
title: FilterColumn.IconFilter
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets IconFilter for filtering data by icon
type: docs
url: /net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

Gets [`IconFilter`](../../iconfilter/) for filtering data by icon.

```csharp
public IconFilter IconFilter { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add sample data with conditional formatting that uses icons
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Apply auto filter to the range
                worksheet.AutoFilter.Range = "A1:A5";

                // Get the filter column
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Access the IconFilter property (read-only)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Display IconFilter properties if it exists
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Save the workbook
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


