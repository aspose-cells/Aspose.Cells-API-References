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
// Called: Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
public static void Property_Name()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the CustomPropertyCollection of the worksheet
            CustomPropertyCollection customProperties = worksheet.CustomProperties;

            // Add custom properties
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            // Access and print the custom properties
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Save the workbook
            workbook.Save("CustomPropertyCollectionExample.xlsx");
            workbook.Save("CustomPropertyCollectionExample.pdf");
            return;
        }
```

### See Also

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


