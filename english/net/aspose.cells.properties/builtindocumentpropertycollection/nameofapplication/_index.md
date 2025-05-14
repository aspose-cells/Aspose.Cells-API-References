---
title: BuiltInDocumentPropertyCollection.NameOfApplication
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the name of the application
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/nameofapplication/
---
## BuiltInDocumentPropertyCollection.NameOfApplication property

Gets or sets the name of the application.

```csharp
public string NameOfApplication { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(!string.IsNullOrEmpty(workbook.BuiltInDocumentProperties.NameOfApplication));
public void BuiltInDocumentPropertyCollection_Property_NameOfApplication()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "SAU Rapporter.ods");
    Assert.IsTrue(!string.IsNullOrEmpty(workbook.BuiltInDocumentProperties.NameOfApplication));
    workbook.Save(Constants.destPath + "example.xml");
    workbook.Save(Constants.destPath + "example.ods");
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


