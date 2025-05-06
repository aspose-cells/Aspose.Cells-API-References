---
title: Worksheet.AddPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Adds page break
type: docs
url: /net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Adds page break.

```csharp
public void AddPageBreaks(string cellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String |  |

### Examples

```csharp
// Called: workbook.Worksheets[0].AddPageBreaks(&amp;quot;B10&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].AddPageBreaks(&quot;B10&quot;);

            workbook.Worksheets[0].AddPageBreaks(&quot;B2&quot;);
            Assert.AreEqual(workbook.Worksheets[0].HorizontalPageBreaks[0].Row, 1);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


