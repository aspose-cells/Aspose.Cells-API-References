---
title: HyperlinkCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: HyperlinkCollection method. Clears all hyperlinks
type: docs
url: /net/aspose.cells/hyperlinkcollection/clear/
---
## HyperlinkCollection.Clear method

Clears all hyperlinks.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Hyperlinks.Clear();
public void HyperlinkCollection_Method_Clear()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.Worksheets[0].Hyperlinks.Clear();
    Assert.AreEqual(TextAlignmentType.General, workbook.Worksheets[0].Cells["A22"].GetStyle().HorizontalAlignment);

}
```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


