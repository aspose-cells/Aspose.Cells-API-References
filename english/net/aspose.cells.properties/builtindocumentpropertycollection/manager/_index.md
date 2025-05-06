---
title: BuiltInDocumentPropertyCollection.Manager
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the manager property
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/manager/
---
## BuiltInDocumentPropertyCollection.Manager property

Gets or sets the manager property.

```csharp
public string Manager { get; set; }
```

### Examples

```csharp
// Called: Manager = &amp;quot;manager&amp;quot;,
[Test]
        public void Property_Manager()
        {
            var wb = new Workbook()
            {
                BuiltInDocumentProperties =
    {
        Author = &quot;author&quot;,
        Title = &quot;title&quot;,
        Comments = &quot;comments&quot;,
        Keywords = &quot;keywords&quot;,
        LastSavedBy = &quot;lastSavedBy&quot;,
        Manager = &quot;manager&quot;,
        Company = &quot;company&quot;,
        Category = &quot;category&quot;,
        Subject = &quot;subject&quot;,
        ContentStatus = &quot;contentStatus&quot;,
        HyperlinkBase = &quot;hyperlinkBase&quot;,
        Template = &quot;template&quot;,
    }
            };

            wb.Settings.Password = &quot;1&quot;;
            wb.Save(Constants.destPath + @&quot;CellsNet56459.xls&quot;, new XlsSaveOptions()
            { EncryptDocumentProperties = true });
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


