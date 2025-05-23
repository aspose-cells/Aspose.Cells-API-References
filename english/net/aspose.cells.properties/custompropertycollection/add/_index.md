---
title: CustomPropertyCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: CustomPropertyCollection method. Adds custom property information
type: docs
url: /net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Adds custom property information.

```csharp
public int Add(string name, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the custom property. |
| value | String | The value of the custom property. |

### Examples

```csharp
// Called: customProperties.Add("Version", "1.0");
public static void CustomPropertyCollection_Method_Add()
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

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


