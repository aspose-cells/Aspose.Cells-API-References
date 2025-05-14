---
title: BuiltInDocumentPropertyCollection.RevisionNumber
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the document revision number
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/revisionnumber/
---
## BuiltInDocumentPropertyCollection.RevisionNumber property

Gets or sets the document revision number.

```csharp
public string RevisionNumber { get; set; }
```

### Remarks

Aspose.Cells does not update this property when you modify the document.

### Examples

```csharp
// Called: Assert.AreEqual("0", workbook.BuiltInDocumentProperties.RevisionNumber);
public void BuiltInDocumentPropertyCollection_Property_RevisionNumber()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xml");
    Assert.AreEqual("0", workbook.BuiltInDocumentProperties.RevisionNumber);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


