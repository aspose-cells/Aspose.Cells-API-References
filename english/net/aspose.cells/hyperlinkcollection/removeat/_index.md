---
title: HyperlinkCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: HyperlinkCollection method. Remove the hyperlink at the specified index in this collection
type: docs
url: /net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Remove the hyperlink at the specified index in this collection.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The zero based index of the element. |

### Examples

```csharp
// Called: sheet.Hyperlinks.RemoveAt(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SpreadsheetWithHyperlinks.xlsm&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Hyperlinks.RemoveAt(0);
            Assert.AreEqual(sheet.Cells[&quot;B3&quot;].GetStyle().Font.Underline, FontUnderlineType.None);
        }
```

### See Also

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


