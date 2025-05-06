---
title: Worksheet.PageSetup
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents the page setup description in this sheet
type: docs
url: /net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Represents the page setup description in this sheet.

```csharp
public PageSetup PageSetup { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(PaperSizeType.Paper10x11, sheet.PageSetup.PaperSize, &amp;quot;sheet.PageSetup.PaperSize&amp;quot;);
private void Property_PageSetup(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            AssertHelper.AreEqual(PaperSizeType.Paper10x11, sheet.PageSetup.PaperSize, &quot;sheet.PageSetup.PaperSize&quot;);
        }
```

### See Also

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


