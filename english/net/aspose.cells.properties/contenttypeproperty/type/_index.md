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
// Called: property.Type = "text";
public static void Property_Type()
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


