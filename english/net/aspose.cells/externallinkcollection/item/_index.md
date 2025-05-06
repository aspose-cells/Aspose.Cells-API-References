---
title: ExternalLinkCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ExternalLinkCollection property. Gets the ExternalLink element at the specified index
type: docs
url: /net/aspose.cells/externallinkcollection/item/
---
## ExternalLinkCollection indexer

Gets the [`ExternalLink`](../../externallink/) element at the specified index.

```csharp
public ExternalLink this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(book.Worksheets.ExternalLinks[0].OriginalDataSource, @&amp;quot;/_Work/Toronto/Parent/parent.xlsx&amp;quot;);
[Test]
        public void Property_Int32_()
        {
            Workbook book = new Workbook(Constants.sourcePath + &quot;CellsNet44402.xlsx&quot;);
            Assert.AreEqual(book.Worksheets.ExternalLinks[0].OriginalDataSource, @&quot;/_Work/Toronto/Parent/parent.xlsx&quot;);
            Console.WriteLine(book.Worksheets.ExternalLinks[0].DataSource);
        }
```

### See Also

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


