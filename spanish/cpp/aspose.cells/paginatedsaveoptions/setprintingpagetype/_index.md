---
title: Aspose::Cells::PaginatedSaveOptions::SetPrintingPageType method
linktitle: SetPrintingPageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPrintingPageType method. Indicates which pages will not be printed in C++.'
type: docs
weight: 2700
url: /es/cpp/aspose.cells/paginatedsaveoptions/setprintingpagetype/
---
## PaginatedSaveOptions::SetPrintingPageType method


Indicates which pages will not be printed.

```cpp
void Aspose::Cells::PaginatedSaveOptions::SetPrintingPageType(PrintingPageType value)
```

## Remarks


If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them. 

## Examples


```cpp
Aspose::Cells::Startup();
//El siguiente código omite páginas en blanco o páginas que solo contienen contenido de estilo como fondo de celda, bordes.
Workbook wb(u"Book1.xlsx");

PdfSaveOptions pdfSaveOptions;

//ignorar páginas en blanco
if (pdfSaveOptions.GetPrintingPageType() != PrintingPageType::IgnoreBlank)
{
    pdfSaveOptions.SetPrintingPageType(PrintingPageType::IgnoreBlank);
}

wb.Save(u"output_ignore_blank_page.pdf", pdfSaveOptions);


//ignorar páginas en blanco y páginas que solo contienen contenido de estilo como fondo de celda
if (pdfSaveOptions.GetPrintingPageType() != PrintingPageType::IgnoreStyle)
{
    pdfSaveOptions.SetPrintingPageType(PrintingPageType::IgnoreStyle);
}

wb.Save(u"output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Enum [PrintingPageType](../../printingpagetype/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
