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
// Called: Assert.IsTrue(workbook.Worksheets.ExternalLinks[0].IsReferred);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44453.xlsx");
            Assert.IsTrue(workbook.Worksheets.ExternalLinks[0].IsReferred);
        }
```

### See Also

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


