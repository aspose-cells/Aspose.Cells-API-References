---
title: Aspose::Cells::PaginatedSaveOptions::SetPrintingPageType method
linktitle: SetPrintingPageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPrintingPageType method. Indicates which pages will not be printed in C++.'
type: docs
weight: 2700
url: /fr/cpp/aspose.cells/paginatedsaveoptions/setprintingpagetype/
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
//Le code suivant omet les pages blanches ou les pages qui ne contiennent que du contenu de style comme le fond de cellule, les bordures.
Workbook wb(u"Book1.xlsx");

PdfSaveOptions pdfSaveOptions;

//ignorer les pages blanches
if (pdfSaveOptions.GetPrintingPageType() != PrintingPageType::IgnoreBlank)
{
    pdfSaveOptions.SetPrintingPageType(PrintingPageType::IgnoreBlank);
}

wb.Save(u"output_ignore_blank_page.pdf", pdfSaveOptions);


//ignorer les pages blanches et les pages qui ne contiennent que du contenu de style comme le fond de cellule
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
