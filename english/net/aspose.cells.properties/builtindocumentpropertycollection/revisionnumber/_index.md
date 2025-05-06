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
// Called: Assert.AreEqual(&amp;quot;8&amp;quot;, workbook.BuiltInDocumentProperties.RevisionNumber);
[Test]
        public void Property_RevisionNumber()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Revision/APP0333.xlsx&quot;);
            Assert.AreEqual(&quot;8&quot;, workbook.BuiltInDocumentProperties.RevisionNumber);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


