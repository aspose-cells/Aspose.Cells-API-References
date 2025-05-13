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
// Called: workbook.Worksheets[0].Hyperlinks[0].TextToDisplay = "test";
public void HyperlinkCollection_Property_Item()
{
    Workbook workbook = new Workbook();

    workbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "www.baidu.com");
    workbook.Worksheets[0].Hyperlinks[0].TextToDisplay = "test";

   AssertHelper.AreEqual(System.Drawing.Color.Blue, workbook.Worksheets[0].Cells["A1"].GetStyle().Font.Color);
    workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[0].Hyperlinks[0].TextToDisplay = "test";
    Assert.AreEqual(20, workbook.Worksheets[0].Cells["B4"].GetStyle().Font.Size);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


