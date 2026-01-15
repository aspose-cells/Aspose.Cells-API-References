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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Create a new CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Display the default And property value
                Console.WriteLine($"Default And property value: {filters.And}");

                // Set the And property to true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // Set the And property to false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Save the workbook
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


