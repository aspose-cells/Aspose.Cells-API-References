---
title: Class AdvancedFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AdvancedFilter class. Represents the settings of the advanced filter
type: docs
url: /net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Represents the settings of the advanced filter.

```csharp
public class AdvancedFilter
```

## Properties

| Name | Description |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Gets the range where copying the resut of this advanced filter to. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Gets the criteria range of this advanced filter. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Gets the list range of this advanced filter. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Populate sample data for the list range
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Populate criteria range
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Get the AdvancedFilter instance from the worksheet
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Display the read-only properties
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Save the workbook
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


