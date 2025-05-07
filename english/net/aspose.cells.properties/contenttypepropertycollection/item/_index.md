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
// Called: Assert.AreEqual(workbook.ContentTypeProperties[0].Name, "ss");
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            workbook.Save(Constants.destPath + "Cellsnet43279.xls");
            workbook = new Workbook(Constants.destPath + "Cellsnet43279.xls");
            Assert.AreEqual(workbook.ContentTypeProperties[0].Name, "ss");
            workbook.Save(Constants.destPath + "Cellsnet43279.xlsx");
            workbook = new Workbook(Constants.destPath + "Cellsnet43279.xlsx");
            Assert.AreEqual(workbook.ContentTypeProperties[0].Name, "ss");
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
public static void Property_String_()
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


