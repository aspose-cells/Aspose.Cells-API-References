---
title: BuiltInDocumentPropertyCollection.ContentType
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the content type of the document
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/contenttype/
---
## BuiltInDocumentPropertyCollection.ContentType property

Gets or sets the content type of the document.

```csharp
public string ContentType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;test_content_type&amp;quot;, wb.BuiltInDocumentProperties.ContentType);
[Test]
        public void Property_ContentType()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsJava42538.xlsx&quot;);
            //Console.WriteLine(wb.BuiltInDocumentProperties.ContentType);
            Assert.AreEqual(&quot;test_content_status&quot;, wb.BuiltInDocumentProperties.ContentStatus);
            Assert.AreEqual(&quot;test_version&quot;, wb.BuiltInDocumentProperties.DocumentVersion);
            // wb.Worksheets[0].ListObjects[0].ConvertToRange();
            // wb.Worksheets[1].ListObjects[0].ConvertToRange();
            Util.ReSave(wb, SaveFormat.Xlsx);
            wb = new Workbook(Constants.sourcePath + &quot;CellsJava42538.xls&quot;);
            Assert.AreEqual(&quot;test_content_type&quot;, wb.BuiltInDocumentProperties.ContentType);
            Assert.AreEqual(&quot;test_content_status&quot;, wb.BuiltInDocumentProperties.ContentStatus);
            Assert.AreEqual(&quot;test_version&quot;, wb.BuiltInDocumentProperties.DocumentVersion);
            // wb.Worksheets[0].ListObjects[0].ConvertToRange();
            // wb.Worksheets[1].ListObjects[0].ConvertToRange();
            Util.ReSave(wb, SaveFormat.Xlsx);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


