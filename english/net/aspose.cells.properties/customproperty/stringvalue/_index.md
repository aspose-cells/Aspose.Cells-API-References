---
title: CustomProperty.StringValue
second_title: Aspose.Cells for .NET API Reference
description: CustomProperty property. Returns or sets the value of the custom property
type: docs
url: /net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Returns or sets the value of the custom property.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use CustomProperty.Value property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a custom property with a string value
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Retrieve the custom property
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // Display the StringValue property (read operation)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // Set a new value for the StringValue property
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Save the workbook
                workbook.Save("StringValueDemo.xlsx");
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


