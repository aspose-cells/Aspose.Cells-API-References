---
title: ContentTypeProperty.Type
second_title: Aspose.Cells for .NET API Reference
description: ContentTypeProperty property. Gets and sets the type of the property
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Gets and sets the type of the property.

```csharp
public string Type { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine("Property Type: " + property.Type);
public static void ContentTypeProperty_Property_Type()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Add a new property to the ContentTypePropertyCollection
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Accessing the ContentTypePropertyCollection
            ContentTypePropertyCollection contentTypeProperties = workbook.ContentTypeProperties;

            // Displaying the count of properties
            Console.WriteLine("Number of ContentTypeProperties: " + contentTypeProperties.Count);

            // Accessing a specific property by index
            ContentTypeProperty property = contentTypeProperties[0];
            Console.WriteLine("Property Name: " + property.Name);
            Console.WriteLine("Property Value: " + property.Value);
            Console.WriteLine("Property Type: " + property.Type);

            // Modifying the capacity of the collection
            contentTypeProperties.Capacity = 10;
            Console.WriteLine("New Capacity: " + contentTypeProperties.Capacity);

            // Save the Excel file
            workbook.Save("ContentTypePropertyCollectionExample.xlsx");
            workbook.Save("ContentTypePropertyCollectionExample.pdf");
        }
```

### See Also

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


