---
title: BuiltInDocumentPropertyCollection.Category
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the category of the document
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

Gets or sets the category of the document.

```csharp
public string Category { get; set; }
```

### Examples

```csharp
// Called: Category = "category",
public void BuiltInDocumentPropertyCollection_Property_Category()
{
    var wb = new Workbook()
{
    BuiltInDocumentProperties =
        {
        Category = "category",
           ContentStatus = "contentStatus",
        }
};

wb.Protect(ProtectionType.All, "p1");
    var xlsStream = new MemoryStream();

wb.Save(xlsStream, SaveFormat.Excel97To2003);
    xlsStream.Position = 0;

    var wb2 = new Workbook(xlsStream);
var bip = wb.BuiltInDocumentProperties;
    Assert.AreEqual("category", bip.Category);
    Assert.AreEqual("contentStatus", bip.ContentStatus);

    var bip2 = wb2.BuiltInDocumentProperties;

    Assert.AreEqual("category", bip2.Category);
    Assert.AreEqual("contentStatus", bip2.ContentStatus);
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


