---
title: CustomFilterCollection.CustomFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: CustomFilterCollection constructor. Constructs new instance
type: docs
url: /net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Constructs new instance.

```csharp
public CustomFilterCollection()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
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
                // Create a new CustomFilterCollection using the constructor
                CustomFilterCollection filters = new CustomFilterCollection();

                // Display the default And property value
                Console.WriteLine($"Default And property value: {filters.And}");

                // The constructor creates an empty collection
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Save the workbook
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


