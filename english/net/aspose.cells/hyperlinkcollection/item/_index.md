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
// Called: Assert.AreEqual(&amp;quot;my-scheme://show/FCD6118F-A863-4977-AD2F-CA56836D9615/0-20?object=3D6DA87D-7B50-47C1-8D5D-80E6173DC117&amp;quot;, links[0].Address);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45946.xlsx&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet45946.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet45946.xlsx&quot;);
            HyperlinkCollection links = workbook.Worksheets[0].Hyperlinks;
            Assert.AreEqual(&quot;my-scheme://show/FCD6118F-A863-4977-AD2F-CA56836D9615/0-20?object=3D6DA87D-7B50-47C1-8D5D-80E6173DC117&quot;, links[0].Address);
            Assert.AreEqual(&quot;myscheme://show/FCD6118F-A863-4977-AD2F-CA56836D9615/0-20?object=3D6DA87D-7B50-47C1-8D5D-80E6173DC117&quot;, links[1].Address);

        }
```

### See Also

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


