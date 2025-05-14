---
title: BuiltInDocumentPropertyCollection.Keywords
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the document keywords
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/keywords/
---
## BuiltInDocumentPropertyCollection.Keywords property

Gets or sets the document keywords.

```csharp
public string Keywords { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, "Testing by Mujeeb");
public void BuiltInDocumentPropertyCollection_Property_Keywords()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.ods");

    Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, "Testing by Mujeeb");
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, "Testing by Mujeeb");
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


