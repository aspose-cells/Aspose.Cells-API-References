---
title: BuiltInDocumentPropertyCollection.LinksUpToDate
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Indicates whether hyperlinks in a document are uptodate
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Indicates whether hyperlinks in a document are up-to-date.

```csharp
public bool LinksUpToDate { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.BuiltInDocumentProperties.LinksUpToDate);
[Test]
        public void Property_LinksUpToDate()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44904.xlsx");
            Assert.IsFalse(workbook.BuiltInDocumentProperties.ScaleCrop);
            Assert.IsFalse(workbook.BuiltInDocumentProperties.LinksUpToDate);
            Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


