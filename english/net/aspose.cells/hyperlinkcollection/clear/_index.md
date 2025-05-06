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
// Called: links.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Hyperlink.xls&quot;);
            HyperlinkCollection links = workbook.Worksheets[0].Hyperlinks;
            links.Clear();
            Style style = workbook.Worksheets[0].Cells[&quot;B1&quot;].GetStyle();
            Assert.AreEqual(style.Font.Color, System.Drawing.Color.Black);
        }
```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


