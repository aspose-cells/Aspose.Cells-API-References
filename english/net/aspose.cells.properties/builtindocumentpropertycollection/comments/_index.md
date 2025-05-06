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
// Called: Assert.AreEqual(&amp;quot;New OMB statement.  Formatted to print on a HP Laser Jet 5si/5si Mx\r\n or HP Laserjet 4...&amp;quot;, builtInDocumentProperties.Comments);
[Test]
        public void Property_Comments()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42686.xlsx&quot;);
            BuiltInDocumentPropertyCollection builtInDocumentProperties = workbook.BuiltInDocumentProperties;
            Assert.AreEqual(&quot;New OMB statement.  Formatted to print on a HP Laser Jet 5si/5si Mx\r\n or HP Laserjet 4...&quot;, builtInDocumentProperties.Comments);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42686.xlsx&quot;);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


