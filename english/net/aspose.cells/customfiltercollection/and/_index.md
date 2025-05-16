---
title: CustomFilterCollection.And
second_title: Aspose.Cells for .NET API Reference
description: CustomFilterCollection property. Indicates whether the two criteria have an and relationship
type: docs
url: /net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

Indicates whether the two criteria have an "and" relationship.

```csharp
public bool And { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.CustomFilterCollectionPropertyAndDemo
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for filtering demonstration
            worksheet.Cells["A1"].Value = "Data";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;

            try
            {
                // Create an AutoFilter for the data range
                worksheet.AutoFilter.Range = "A1:A5";
                
                // Apply custom filtering directly using the Custom method
                worksheet.AutoFilter.Custom(0, FilterOperatorType.Equal, 10);
                worksheet.AutoFilter.Custom(0, FilterOperatorType.Equal, 40, true, FilterOperatorType.Equal, 40);
                
                // Display the current And value (not directly accessible in this approach)
                Console.WriteLine("Using AND logic for filters");
                
                // Apply the filter (this would normally hide non-matching rows)
                worksheet.AutoFilter.Refresh();
                
                // Save the workbook
                workbook.Save("AndDemo.xlsx");
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

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


