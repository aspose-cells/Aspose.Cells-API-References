---
title: BuiltInDocumentPropertyCollection.Version
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Represents the version number of the application that created the document
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/version/
---
## BuiltInDocumentPropertyCollection.Version property

Represents the version number of the application that created the document.

```csharp
public string Version { get; set; }
```

### Remarks

It's format is "00.0000",for example : 12.0000

### Examples

```csharp
// Called: Assert.AreEqual("14.0300", workbook.Worksheets.BuiltInDocumentProperties.Version);
public void BuiltInDocumentPropertyCollection_Property_Version()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    Assert.AreEqual("14.0300", workbook.Worksheets.BuiltInDocumentProperties.Version);
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


