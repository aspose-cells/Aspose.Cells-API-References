---
title: HyperlinkCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: HyperlinkCollection property. Gets the Hyperlink element at the specified index
type: docs
url: /net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Gets the [`Hyperlink`](../../hyperlink/) element at the specified index.

```csharp
public Hyperlink this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: book.Worksheets[0].Hyperlinks[x].TextToDisplay = "Test link";
[Test]
        public void Property_Int32_()
        {
            Console.WriteLine("Property_Int32_()");
            string outfn = Constants.destPath + "Test_HrefLinkedText_out.xlsx";

            Workbook book = new Workbook();

            int x = book.Worksheets[0].Hyperlinks.Add(1, 1, 1, 1, "'Class1'!A1");
            book.Worksheets[0].Hyperlinks[x].TextToDisplay = "Test link";

            book.Save(outfn);
        }
```

### See Also

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


