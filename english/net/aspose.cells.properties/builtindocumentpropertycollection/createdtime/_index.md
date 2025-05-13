---
title: BuiltInDocumentPropertyCollection.CreatedTime
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets date of the document creation in local timezone
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/createdtime/
---
## BuiltInDocumentPropertyCollection.CreatedTime property

Gets or sets date of the document creation in local timezone.

```csharp
public DateTime CreatedTime { get; set; }
```

### Remarks

Aspose.Cells does not update this property when you modify the document.

### Examples

```csharp
// Called: Assert.AreEqual(dt.Hour, workbook.BuiltInDocumentProperties.CreatedTime.Hour);
public void BuiltInDocumentPropertyCollection_Property_CreatedTime()
{
    Workbook workbook = new Workbook();
    DateTime dt = DateTime.Now;
    workbook.BuiltInDocumentProperties.CreatedTime = dt;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(dt.Hour, workbook.BuiltInDocumentProperties.CreatedTime.Hour);
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


