---
title: BuiltInDocumentPropertyCollection.HyperlinkBase
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the hyperlinkbase property
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/hyperlinkbase/
---
## BuiltInDocumentPropertyCollection.HyperlinkBase property

Gets or sets the hyperlinkbase property.

```csharp
public string HyperlinkBase { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets.BuiltInDocumentProperties.HyperlinkBase, "http://www.svd.se");
[Test]
        public void Property_HyperlinkBase()
        {
            Workbook workbook = new Workbook();
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.svd.se"; // This has no effect

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "SomeTitle"; // This sets the Title.

            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            Assert.AreEqual(workbook.Worksheets.BuiltInDocumentProperties.HyperlinkBase, "http://www.svd.se");
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


