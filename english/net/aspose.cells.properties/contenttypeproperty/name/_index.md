---
title: ContentTypeProperty.Name
second_title: Aspose.Cells for .NET API Reference
description: ContentTypeProperty property. Returns or sets the name of the object
type: docs
url: /net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Returns or sets the name of the object.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.ContentTypeProperties[0].Name, "ss");
public void ContentTypeProperty_Property_Name()
{
    Workbook workbook = new Workbook();
    workbook.ContentTypeProperties.Add("ss", "bb", "text");
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(workbook.ContentTypeProperties[0].Name, "ss");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(workbook.ContentTypeProperties[0].Name, "ss");
}
```

### See Also

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


