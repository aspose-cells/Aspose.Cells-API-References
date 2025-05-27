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
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the custom properties collection
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Add custom properties with names and values
            DocumentProperty prop1 = customProperties.Add("Author", "John Doe");
            DocumentProperty prop2 = customProperties.Add("Version", "1.0");
            DocumentProperty prop3 = customProperties.Add("CreatedDate", DateTime.Now.ToString());
            
            // Display the custom properties using the Name property
            Console.WriteLine("Custom Properties:");
            foreach (DocumentProperty prop in customProperties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}");
            }
            
            // Access a property by name
            DocumentProperty authorProp = customProperties["Author"];
            if (authorProp != null)
            {
                Console.WriteLine($"\nAuthor property value: {authorProp.Value}");
            }
        }
    }
}
```

### See Also

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


