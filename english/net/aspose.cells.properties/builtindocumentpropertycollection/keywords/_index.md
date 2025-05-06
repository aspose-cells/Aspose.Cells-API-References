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
// Called: Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, &amp;quot;Testing by Mujeeb&amp;quot;);
[Test]
        public void Property_Keywords()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet42900.ods&quot;);

            Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, &quot;Testing by Mujeeb&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet42900.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet42900.ods&quot;);
            Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, &quot;Testing by Mujeeb&quot;);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


