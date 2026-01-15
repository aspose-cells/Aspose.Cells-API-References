---
title: FilterColumn.DynamicFilter
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets DynamicFilter for filtering with dynamic criteria
type: docs
url: /net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Gets [`DynamicFilter`](../../dynamicfilter/) for filtering with dynamic criteria.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add sample data
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Apply auto filter
                worksheet.AutoFilter.Range = "A1:A4";

                // Get the filter column
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Access the DynamicFilter property (read-only)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // Display DynamicFilter properties
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Save the workbook
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


