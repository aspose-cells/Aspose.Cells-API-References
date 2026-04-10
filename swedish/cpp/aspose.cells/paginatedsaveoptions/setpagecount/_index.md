---
title: Aspose::Cells::PaginatedSaveOptions::SetPageCount method
linktitle: SetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2400
url: /sv/cpp/aspose.cells/paginatedsaveoptions/setpagecount/
---
## PaginatedSaveOptions::SetPageCount method


Gets or sets the number of pages to save.

```cpp
void Aspose::Cells::PaginatedSaveOptions::SetPageCount(int32_t value)
```

## Remarks


Default is System.Int32.MaxValue which means all pages will be rendered.. 

## Examples


```cpp
Aspose::Cells::Startup();
//Följande exempel visar hur man renderar ett intervall av sidor (3 och 4) i en Microsoft Excel-fil till PDF.
 //Öppna en Excel-fil
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Skriv ut endast sida 3 och sida 4 i den genererade PDF-filen
//Startsidindex (0-baserat index)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Antal sidor som ska skrivas ut
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//Spara PDF-filen
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
