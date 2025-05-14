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
public void BuiltInDocumentPropertyCollection_Property_Subject()
{
    var filePath = Constants.sourcePath + "example.xlsx";
    using (var wb = new Workbook(filePath, new LoadOptions(LoadFormat.Xlsx)
    {
        Password = "1",
    }))
    {
        // t and s are empty string
        var t = wb.BuiltInDocumentProperties.Title;//empty string
        var s = wb.BuiltInDocumentProperties.Subject;//empty string
        Assert.AreEqual("LiteraTest", t);
        Assert.AreEqual("LiteraTest", s);
    }
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


