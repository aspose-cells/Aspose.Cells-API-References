---
title: BuiltInDocumentPropertyCollection.ScaleCrop
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Indicates the display mode of the document thumbnail
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

Indicates the display mode of the document thumbnail.

```csharp
public bool ScaleCrop { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.BuiltInDocumentProperties.ScaleCrop);
[Test]
        public void Property_ScaleCrop()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44904.xlsx&quot;);
            Assert.IsFalse(workbook.BuiltInDocumentProperties.ScaleCrop);
            Assert.IsFalse(workbook.BuiltInDocumentProperties.LinksUpToDate);
            Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


