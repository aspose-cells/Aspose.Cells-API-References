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
// Called: sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;
[Test]
        public void Property_PaperSize()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            checkPaperSizeType_PaperLetter(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkPaperSizeType_PaperLetter(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkPaperSizeType_PaperLetter(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
            checkPaperSizeType_PaperLetter(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


