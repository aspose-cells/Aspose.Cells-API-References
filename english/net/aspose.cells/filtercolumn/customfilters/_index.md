---
title: FilterColumn.CustomFilters
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets CustomFilterCollection for filtering data by custom criteria
type: docs
url: /net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

Gets [`CustomFilterCollection`](../../customfiltercollection/) for filtering data by custom criteria.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add sample data
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Apply auto filter
                worksheet.AutoFilter.Range = "A1:A6";

                // Get the filter column
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Create and set custom filters using AutoFilter.Custom method
                // First filter: begins with "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // Second filter: ends with "y" (AND relationship)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Get the custom filters from the filter column
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Display the custom filters information
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Note: CustomFilterCollection doesn't expose individual filters directly
                // through an indexer, so we can only display the collection properties
                Console.WriteLine("Custom filters have been applied to the column.");

                // Save the workbook
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


