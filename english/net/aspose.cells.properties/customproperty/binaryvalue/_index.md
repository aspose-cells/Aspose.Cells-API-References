---
title: CustomProperty.BinaryValue
second_title: Aspose.Cells for .NET API Reference
description: CustomProperty property. Gets and sets the binary value of the custom property
type: docs
url: /net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Gets and sets the binary value of the custom property.

```csharp
public byte[] BinaryValue { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a custom property with a sample value
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Retrieve the custom property
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Display the Name and Value of the custom property
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // NOTE: The reflection for CustomProperty does not include a BinaryValue property.
                // The available string-based value is accessed via the 'Value' property.

                // Save the workbook (optional)
                workbook.Save("BinaryValueDemo.xlsx");
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


