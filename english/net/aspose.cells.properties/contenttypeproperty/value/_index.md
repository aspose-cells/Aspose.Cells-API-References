---
title: ContentTypeProperty.Value
second_title: Aspose.Cells for .NET API Reference
description: ContentTypeProperty property. Returns or sets the value of the content type property
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

Returns or sets the value of the content type property.

```csharp
public string Value { get; set; }
```

### Examples

```csharp
// Called: property.Value = &amp;quot;Aspose&amp;quot;;
public static void Property_Value()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Add a new content type property
            workbook.ContentTypeProperties.Add(&quot;Admin&quot;, &quot;Aspose&quot;, &quot;text&quot;);

            // Access the newly added property
            ContentTypeProperty property = workbook.ContentTypeProperties[&quot;Admin&quot;];
            
            // Setting properties
            property.Name = &quot;Admin&quot;;
            property.Value = &quot;Aspose&quot;;
            property.Type = &quot;text&quot;;
            property.IsNillable = true;

            // Save the Excel file
            workbook.Save(&quot;ContentTypePropertyExample.xlsx&quot;);
            workbook.Save(&quot;ContentTypePropertyExample.pdf&quot;);
            return;
        }
```

### See Also

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


