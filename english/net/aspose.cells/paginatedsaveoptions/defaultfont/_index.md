---
title: PaginatedSaveOptions.DefaultFont
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set Aspose.Cells will use system default font to show these unicode characters
type: docs
url: /net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```csharp
public string DefaultFont { get; set; }
```

### Examples

```csharp
// Called: pdfSaveOptions.DefaultFont = "宋体";
[Test]
        public void Property_DefaultFont()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet52420.xls");
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
            pdfwb.Save(Constants.destPath + "CellsNet52420.pdf");
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


