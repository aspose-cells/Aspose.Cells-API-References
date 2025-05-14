---
title: ContentTypeProperty.IsNillable
second_title: Aspose.Cells for .NET API Reference
description: ContentTypeProperty property. Indicates whether the value could be empty
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Indicates whether the value could be empty.

```csharp
public bool IsNillable { get; set; }
```

### Examples

```csharp
// Called: property.IsNillable = true;
public static void ContentTypeProperty_Property_IsNillable()
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


