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
// Called: Console.WriteLine("Original Data Source:" + workbook.Worksheets.ExternalLinks[i].OriginalDataSource);
        public void ExternalLinkCollection_Property_Item()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
            //for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            int i = 1;
            {
                Console.WriteLine((i + 1).ToString() + ". " + workbook.Worksheets.ExternalLinks[i].DataSource);
#if !LINUX_TEST
                Assert.IsTrue(workbook.Worksheets.ExternalLinks[i].DataSource.StartsWith("S:"));
                Console.WriteLine("Original Data Source:" + workbook.Worksheets.ExternalLinks[i].OriginalDataSource);
                //Console.WriteLine("ToString:" + workbook.Worksheets.ExternalLinks[i].ToString());
#endif
            }
        }
```

### See Also

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


