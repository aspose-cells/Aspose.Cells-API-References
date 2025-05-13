---
title: ContentTypePropertyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ContentTypePropertyCollection property. Gets the content type property by the specific index
type: docs
url: /net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Gets the content type property by the specific index.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

The content type property

### Examples

```csharp
// Called: workbook.ContentTypeProperties[index].IsNillable = true;
public void ContentTypePropertyCollection_Property_Item()
{
    Workbook workbook = new Workbook(FileFormatType.Xlsx);
    int index = workbook.ContentTypeProperties.Add("MK31", "Simple Data");
    workbook.ContentTypeProperties[index].IsNillable = true;
    //index= workbook.ContentTypeProperties.Add("MK32", "2019-10-17T16:00:00+00:00", "DateTime");
    index = workbook.ContentTypeProperties.Add("MK32",
        DateTime.Now.ToString("yyyy-MM-dd'T'hh:mm:ss"), "DateTime");
    workbook.ContentTypeProperties[index].IsNillable = true;
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Gets the content type property by the property name.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The property name. |

### Return Value

The content type property

### Examples

```csharp
// Called: ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
public static void ContentTypePropertyCollection_Property_Item()
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

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


