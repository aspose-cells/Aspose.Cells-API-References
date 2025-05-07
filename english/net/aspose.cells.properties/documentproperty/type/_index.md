---
title: DocumentProperty.Type
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty property. Gets the data type of the property
type: docs
url: /net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

Gets the data type of the property.

```csharp
public PropertyType Type { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
public static void Property_Type()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the built-in document properties
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Set some built-in properties
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demonstration of PropertyType";
            builtInProperties.Company = "Aspose";

            // Access the custom document properties
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Add custom properties of different types
            customProperties.Add("IsReviewed", true); // Boolean
            customProperties.Add("ReviewDate", DateTime.Now); // DateTime
            customProperties.Add("Rating", 4.5); // Double
            customProperties.Add("Pages", 100); // Number
            customProperties.Add("Summary", "This is a sample workbook for demonstrating PropertyType."); // String

            // Retrieve and display custom properties
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Save the workbook
            workbook.Save("PropertyTypeExample.xlsx");
        }
```

### See Also

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


