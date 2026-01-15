---
title: CustomProperty.Name
second_title: Aspose.Cells for .NET API Reference
description: CustomProperty property. Returns or sets the name of the object
type: docs
url: /net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Returns or sets the name of the object.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a custom property with a name and value
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Retrieve the custom property
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Display the current value of the Name property (read operation)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Set a new value for the Name property
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Save the workbook
                workbook.Save("NameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


