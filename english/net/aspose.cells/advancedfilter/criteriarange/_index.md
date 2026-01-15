---
title: AdvancedFilter.CriteriaRange
second_title: Aspose.Cells for .NET API Reference
description: AdvancedFilter property. Gets the criteria range of this advanced filter
type: docs
url: /net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Gets the criteria range of this advanced filter.

```csharp
public string CriteriaRange { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Populate sample data for the list range
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Populate sample criteria (the filter will use this when applied)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // Obtain the AdvancedFilter object for the worksheet
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // The ListRange, CriteriaRange and CopyToRange properties are read‑only.
                // Display the automatically determined ranges.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Save the workbook (optional, just to show the file can be created)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


