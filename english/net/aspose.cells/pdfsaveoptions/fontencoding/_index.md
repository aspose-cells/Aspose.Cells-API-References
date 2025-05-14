---
title: PdfSaveOptions.FontEncoding
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets or sets embedded font encoding in pdf
type: docs
url: /net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

Gets or sets embedded font encoding in pdf.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Remarks

Default value is Identity

### Examples

```csharp
// Called: pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;
public void PdfSaveOptions_Property_FontEncoding()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    // workbook.Save(dir + "dest.pdf");
    Worksheet worksheet = workbook.Worksheets[0];

    Workbook pdfwb = new Workbook();

    for (int i = pdfwb.Worksheets.Count; i > 0; i--)
    {
        pdfwb.Worksheets.RemoveAt(i - 1);
    }
    if (worksheet.IsVisible == true)
    {
        int s = pdfwb.Worksheets.Add();
        pdfwb.Worksheets[s].Copy(worksheet);
    }

    PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
    pdfSaveOptions.OnePagePerSheet = true;
    pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;
    pdfSaveOptions.DefaultFont = "宋体";
    pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
    pdfSaveOptions.CheckWorkbookDefaultFont = true;
    pdfwb.Save(Constants.destPath + "example.pdf");
}
```

### See Also

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


