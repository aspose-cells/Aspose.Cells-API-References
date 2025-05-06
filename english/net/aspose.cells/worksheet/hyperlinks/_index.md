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
// Called: HyperlinkCollection links = excel.Worksheets[1].Hyperlinks;
[Test]
        public void Property_Hyperlinks()
        {
            Workbook excel = new Workbook(Constants.sourcePath + &quot;CELLSNET49015.xlsx&quot;);
            excel.Worksheets[0].Name = &quot;abcd&quot;;
            HyperlinkCollection links = excel.Worksheets[1].Hyperlinks;
            Assert.AreEqual(&quot;abcd!C3&quot;,links[0].Address);
            Assert.AreEqual(&quot;http://www.google.com/&quot;,links[1].Address);
            Assert.AreEqual(&quot;12345.xlsx&quot;,links[2].Address);
        }
```

### See Also

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


