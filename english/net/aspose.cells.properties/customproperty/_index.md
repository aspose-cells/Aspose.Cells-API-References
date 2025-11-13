---
title: Class CustomProperty
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Properties.CustomProperty class. Represents a custom property which store name and value pairs of arbitrary userdefined data for worksheet
type: docs
url: /net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Represents a custom property which store name and value pairs of arbitrary user-defined data for worksheet.

```csharp
public class CustomProperty
```

## Properties

| Name | Description |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Gets and sets the binary value of the custom property. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Returns or sets the name of the object. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) Returns or sets the value of the custom property. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Returns or sets the value of the custom property. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Access the CustomProperties collection
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Add custom properties
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Access and display custom properties
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Save the workbook
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


