---
title: BuiltInDocumentPropertyCollection.Subject
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the subject of the document
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/subject/
---
## BuiltInDocumentPropertyCollection.Subject property

Gets or sets the subject of the document.

```csharp
public string Subject { get; set; }
```

### Examples

```csharp
// Called: var s = wb.BuiltInDocumentProperties.Subject;//empty string
[Test]
        public void Property_Subject()
        {
            var filePath = Constants.sourcePath + &quot;CellsNet56334.xlsx&quot;;
            using (var wb = new Workbook(filePath, new LoadOptions(LoadFormat.Xlsx)
            {
                Password = &quot;1&quot;,
            }))
            {
                // t and s are empty string
                var t = wb.BuiltInDocumentProperties.Title;//empty string
                var s = wb.BuiltInDocumentProperties.Subject;//empty string
                Assert.AreEqual(&quot;LiteraTest&quot;, t);
                Assert.AreEqual(&quot;LiteraTest&quot;, s);
            }
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


