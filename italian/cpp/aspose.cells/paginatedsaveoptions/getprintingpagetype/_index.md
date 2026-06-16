---
title: Aspose::Cells::PaginatedSaveOptions::GetPrintingPageType method
linktitle: GetPrintingPageType
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetPrintingPageType method. Indicates which pages will not be printed in C++.'
type: docs
weight: 2600
url: /it/cpp/aspose.cells/paginatedsaveoptions/getprintingpagetype/
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
//Il codice seguente omette le pagine vuote o le pagine che contengono solo contenuti di stile come lo sfondo delle celle, i bordi.
Workbook wb(u"Book1.xlsx");

PdfSaveOptions pdfSaveOptions;

//ignora le pagine vuote
if (pdfSaveOptions.GetPrintingPageType() != PrintingPageType::IgnoreBlank)
{
    pdfSaveOptions.SetPrintingPageType(PrintingPageType::IgnoreBlank);
}

wb.Save(u"output_ignore_blank_page.pdf", pdfSaveOptions);


//ignora le pagine vuote e le pagine che contengono solo contenuti di stile come lo sfondo delle celle
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
