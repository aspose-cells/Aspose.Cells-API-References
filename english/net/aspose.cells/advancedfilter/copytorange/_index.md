---
title: AdvancedFilter.CopyToRange
second_title: Aspose.Cells for .NET API Reference
description: AdvancedFilter property. Gets the range where copying the resut of this advanced filter to
type: docs
url: /net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Gets the range where copying the resut of this advanced filter to.

```csharp
public string CopyToRange { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Get the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // Add criteria range
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // Get the AdvancedFilter instance from the worksheet
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Display the CopyToRange property value
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // Save the workbook
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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


