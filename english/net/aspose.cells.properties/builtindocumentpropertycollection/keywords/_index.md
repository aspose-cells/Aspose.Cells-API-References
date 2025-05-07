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
[Test]
        public void Property_Keywords()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet42900.ods");

            Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, "Testing by Mujeeb");
            workbook.Save(Constants.destPath + "CellsNet42900.ods");
            workbook = new Workbook(Constants.destPath + "CellsNet42900.ods");
            Assert.AreEqual(workbook.BuiltInDocumentProperties.Keywords, "Testing by Mujeeb");
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


