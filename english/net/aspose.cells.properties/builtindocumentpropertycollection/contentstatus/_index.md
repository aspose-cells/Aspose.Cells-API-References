---
title: BuiltInDocumentPropertyCollection.ContentStatus
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the content status of the document
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/contentstatus/
---
## BuiltInDocumentPropertyCollection.ContentStatus property

Gets or sets the content status of the document.

```csharp
public string ContentStatus { get; set; }
```

### Examples

```csharp
// Called: ContentStatus = "contentStatus",
    public void BuiltInDocumentPropertyCollection_Property_ContentStatus()
    {
        var wb = new Workbook()
        {
            BuiltInDocumentProperties =
{
    Author = "author",
    Title = "title",
    Comments = "comments",
    Keywords = "keywords",
    LastSavedBy = "lastSavedBy",
    Manager = "manager",
    Company = "company",
    Category = "category",
    Subject = "subject",
    ContentStatus = "contentStatus",
    HyperlinkBase = "hyperlinkBase",
    Template = "template",
}
        };

        wb.Settings.Password = "1";
        wb.Save(Constants.destPath + @"example.xls", new XlsSaveOptions()
        { EncryptDocumentProperties = true });
    }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


