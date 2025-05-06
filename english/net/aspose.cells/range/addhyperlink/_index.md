---
title: Range.AddHyperlink
second_title: Aspose.Cells for .NET API Reference
description: Range method. Adds a hyperlink to a specified cell or a range of cells
type: docs
url: /net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Adds a hyperlink to a specified cell or a range of cells.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |

### Return Value

[`Hyperlink`](../../hyperlink/) object.

### Examples

```csharp
// Called: r.AddHyperlink(&amp;quot;www.aspose.com&amp;quot;, &amp;quot;www.aspose.com&amp;quot;, &amp;quot;www.aspose.com&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range r = sheet.Cells.CreateRange(&quot;A1:A10&quot;);
            r.AddHyperlink(&quot;www.aspose.com&quot;, &quot;www.aspose.com&quot;, &quot;www.aspose.com&quot;);
            Assert.AreEqual(&quot;www.aspose.com&quot;, sheet.Hyperlinks[0].TextToDisplay);

        }
```

### See Also

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


