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
// Called: Console.WriteLine(&amp;quot;Property Type: &amp;quot; + property.Type);
public static void Property_Type()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Add a new property to the ContentTypePropertyCollection
            workbook.ContentTypeProperties.Add(&quot;Admin&quot;, &quot;Aspose&quot;, &quot;text&quot;);

            // Accessing the ContentTypePropertyCollection
            ContentTypePropertyCollection contentTypeProperties = workbook.ContentTypeProperties;

            // Displaying the count of properties
            Console.WriteLine(&quot;Number of ContentTypeProperties: &quot; + contentTypeProperties.Count);

            // Accessing a specific property by index
            ContentTypeProperty property = contentTypeProperties[0];
            Console.WriteLine(&quot;Property Name: &quot; + property.Name);
            Console.WriteLine(&quot;Property Value: &quot; + property.Value);
            Console.WriteLine(&quot;Property Type: &quot; + property.Type);

            // Modifying the capacity of the collection
            contentTypeProperties.Capacity = 10;
            Console.WriteLine(&quot;New Capacity: &quot; + contentTypeProperties.Capacity);

            // Save the Excel file
            workbook.Save(&quot;ContentTypePropertyCollectionExample.xlsx&quot;);
            workbook.Save(&quot;ContentTypePropertyCollectionExample.pdf&quot;);
        }
```

### See Also

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


