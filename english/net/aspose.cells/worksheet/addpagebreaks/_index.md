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
// Called: workbook.Worksheets[0].AddPageBreaks("B10");
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].AddPageBreaks("B10");

            workbook.Worksheets[0].AddPageBreaks("B2");
            Assert.AreEqual(workbook.Worksheets[0].HorizontalPageBreaks[0].Row, 1);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


