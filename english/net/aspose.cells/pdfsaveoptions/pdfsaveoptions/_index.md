---
title: PdfSaveOptions.PdfSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions constructor. Creates the options for saving pdf file
type: docs
url: /net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Creates the options for saving pdf file.

```csharp
public PdfSaveOptions()
```

### Examples

```csharp
// Called: Aspose.Cells.PdfSaveOptions opts = new Aspose.Cells.PdfSaveOptions();
[Test]
        public void PdfSaveOptions_Constructor()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet46449.xlsx");
            string tag = "REV_NO$DOC_KODU";
            string replace = "1$ys";

            for (int i = 0; i < tag.Split('$').Length; i++)
            {
                sheetReplace(wb, "<" + tag.Split('$')[i] + ">", replace.Split('$')[i]);
            }
            Aspose.Cells.PdfSaveOptions opts = new Aspose.Cells.PdfSaveOptions();

            wb.Save(Constants.destPath + "CellsNet46449.pdf", opts);

        }
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


