---
title: FilterColumn.MultipleFilters
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets MultipleFilterCollection for filtering data by labels or date time
type: docs
url: /net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

Gets [`MultipleFilterCollection`](../../multiplefiltercollection/) for filtering data by labels or date time.

```csharp
public MultipleFilterCollection MultipleFilters { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add sample data
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // Apply AutoFilter to the range
                worksheet.AutoFilter.Range = "A1:A5";

                // Get the first filter column
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Create and set MultipleFilters
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // Assign the MultipleFilters to the filter column
                filterColumn.MultipleFilters = multipleFilters;

                // Display the MultipleFilters properties
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // Save the workbook
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


