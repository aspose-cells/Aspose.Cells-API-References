---
title: BuiltInDocumentPropertyCollection.Comments
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the document comments
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/comments/
---
## BuiltInDocumentPropertyCollection.Comments property

Gets or sets the document comments.

```csharp
public string Comments { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("New OMB statement.  Formatted to print on a HP Laser Jet 5si/5si Mx\r\n or HP Laserjet 4...", builtInDocumentProperties.Comments);
public void BuiltInDocumentPropertyCollection_Property_Comments()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    BuiltInDocumentPropertyCollection builtInDocumentProperties = workbook.BuiltInDocumentProperties;
    Assert.AreEqual("New OMB statement.  Formatted to print on a HP Laser Jet 5si/5si Mx\r\n or HP Laserjet 4...", builtInDocumentProperties.Comments);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


