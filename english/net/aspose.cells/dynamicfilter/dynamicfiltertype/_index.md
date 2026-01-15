---
title: DynamicFilter.DynamicFilterType
second_title: Aspose.Cells for .NET API Reference
description: DynamicFilter property. Gets and sets the type of this dynamic filter
type: docs
url: /net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Gets and sets the type of this dynamic filter.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data with dates
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Create auto filter
                worksheet.AutoFilter.Range = "A1:A5";

                // Apply dynamic filter for March dates
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // Get the DynamicFilter instance
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Display the current DynamicFilterType value
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Change the filter type to show April dates
                filter.DynamicFilterType = DynamicFilterType.April;

                // Display the updated DynamicFilterType value
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Apply the filter
                worksheet.AutoFilter.Refresh();

                // Save the result
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
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

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


