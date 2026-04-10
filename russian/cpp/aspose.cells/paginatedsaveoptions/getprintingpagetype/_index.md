---
title: Aspose::Cells::PaginatedSaveOptions::GetPrintingPageType method
linktitle: GetPrintingPageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetPrintingPageType method. Indicates which pages will not be printed in C++.'
type: docs
weight: 2600
url: /ru/cpp/aspose.cells/paginatedsaveoptions/getprintingpagetype/
---
## PaginatedSaveOptions::GetPrintingPageType method


Indicates which pages will not be printed.

```cpp
PrintingPageType Aspose::Cells::PaginatedSaveOptions::GetPrintingPageType()
```

## Remarks


If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them. 

## Examples


```cpp
Aspose::Cells::Startup();
//Следующий код пропускает пустые страницы или страницы, содержащие только стилистическое содержимое, например фон ячеек, границы.
Workbook wb(u"Book1.xlsx");

PdfSaveOptions pdfSaveOptions;

//игнорировать пустые страницы
if (pdfSaveOptions.GetPrintingPageType() != PrintingPageType::IgnoreBlank)
{
    pdfSaveOptions.SetPrintingPageType(PrintingPageType::IgnoreBlank);
}

wb.Save(u"output_ignore_blank_page.pdf", pdfSaveOptions);


//игнорировать пустые страницы и страницы, содержащие только стилистическое содержимое, например фон ячеек
if (pdfSaveOptions.GetPrintingPageType() != PrintingPageType::IgnoreStyle)
{
    pdfSaveOptions.SetPrintingPageType(PrintingPageType::IgnoreStyle);
}

wb.Save(u"output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Enum [PrintingPageType](../../printingpagetype/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
