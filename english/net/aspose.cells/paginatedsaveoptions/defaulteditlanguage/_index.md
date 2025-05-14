---
title: PaginatedSaveOptions.DefaultEditLanguage
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Gets or sets default edit language
type: docs
url: /net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

Gets or sets default edit language.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Remarks

It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.

### Examples

```csharp
// Called: pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
public void PaginatedSaveOptions_Property_DefaultEditLanguage()
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

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


