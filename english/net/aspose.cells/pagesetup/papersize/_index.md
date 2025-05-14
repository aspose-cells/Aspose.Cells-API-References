---
title: PageSetup.PaperSize
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the paper
type: docs
url: /net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Represents the size of the paper.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(PaperSizeType.PaperEnvelopeB6, sheet.PageSetup.PaperSize, "sheet.PageSetup.PaperSize");
private void PageSetup_Property_PaperSize(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            AssertHelper.AreEqual(PaperSizeType.PaperEnvelopeB6, sheet.PageSetup.PaperSize, "sheet.PageSetup.PaperSize");
        }
```

### See Also

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


