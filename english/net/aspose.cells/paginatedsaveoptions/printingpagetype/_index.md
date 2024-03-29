---
title: PaginatedSaveOptions.PrintingPageType
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Indicates which pages will not be printed
type: docs
url: /net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Indicates which pages will not be printed.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Remarks

If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

### Examples

The following code omits blank pages or pages which only contains some style content like cell background, borders.

```csharp
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//ignore blank pages
pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);


//ignore blank pages and pages which only contains some style content like cell background
pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

### See Also

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


