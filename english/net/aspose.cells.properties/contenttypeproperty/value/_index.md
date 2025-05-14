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
// Called: property.Value = "Aspose";
public static void ContentTypeProperty_Property_Value()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Add a new content type property
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Access the newly added property
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Setting properties
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Save the Excel file
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
```

### See Also

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


