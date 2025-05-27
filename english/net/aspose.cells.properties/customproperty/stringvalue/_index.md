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
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a custom property
            DocumentProperty customProperty = workbook.CustomDocumentProperties.Add("AuthorInfo", "John Doe");

            // Display the current StringValue (obsolete, shown for demonstration)
            Console.WriteLine("Current StringValue (obsolete): " + customProperty.Value.ToString());

            // Display the current Value (recommended property)
            Console.WriteLine("Current Value: " + customProperty.Value);

            // Set a new value using the recommended property
            customProperty.Value = "Jane Smith";

            // Verify the change
            Console.WriteLine("Updated Value: " + customProperty.Value);

            // Demonstrate usage in spreadsheet
            worksheet.Cells["A1"].PutValue("Document Author:");
            worksheet.Cells["B1"].PutValue(customProperty.Value);

            // Save the result
            workbook.Save("PropertyStringValueDemo.xlsx");
        }
    }
}
```

### See Also

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


