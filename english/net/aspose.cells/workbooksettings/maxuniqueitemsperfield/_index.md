---
title: WorkbookSettings.MaxUniqueItemsPerField
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and set the limitation of unique items per field
type: docs
url: /net/aspose.cells/workbooksettings/maxuniqueitemsperfield/
---
## WorkbookSettings.MaxUniqueItemsPerField property

Gets and set the limitation of unique items per field

```csharp
public int MaxUniqueItemsPerField { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertyMaxUniqueItemsPerFieldDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            try
            {
                // Display the current MaxUniqueItemsPerField value
                Console.WriteLine("Current MaxUniqueItemsPerField value: " + settings.MaxUniqueItemsPerField);

                // Demonstrate setting a new value for MaxUniqueItemsPerField
                settings.MaxUniqueItemsPerField = 1000;
                Console.WriteLine("After setting to 1000: " + settings.MaxUniqueItemsPerField);

                // Set another value to show it's mutable
                settings.MaxUniqueItemsPerField = 5000;
                Console.WriteLine("After setting to 5000: " + settings.MaxUniqueItemsPerField);

                // Add some sample data to make the example meaningful
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Orange");

                // Save the workbook
                workbook.Save("MaxUniqueItemsPerFieldDemo.xlsx");
                Console.WriteLine("Workbook saved with MaxUniqueItemsPerField settings.");
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

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


