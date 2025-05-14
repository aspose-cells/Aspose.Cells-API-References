---
title: Worksheet.Hyperlinks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the HyperlinkCollection collection
type: docs
url: /net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Gets the [`HyperlinkCollection`](../../hyperlinkcollection/) collection.

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Hyperlinks.Add(0, 0, 1, 1, @"d:\_Work\whatever\Test.docx");
public void Worksheet_Property_Hyperlinks()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].Hyperlinks.Add(0, 0, 1, 1, @"d:\_Work\whatever\Test.docx");

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(@"d:\_Work\whatever\Test.docx", workbook.Worksheets[0].Hyperlinks[0].Address);
}
```

### See Also

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


