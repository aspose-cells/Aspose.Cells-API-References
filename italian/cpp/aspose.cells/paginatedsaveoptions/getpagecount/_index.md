---
title: Aspose::Cells::PaginatedSaveOptions::GetPageCount method
linktitle: GetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2500
url: /it/cpp/aspose.cells/paginatedsaveoptions/getpagecount/
---
## PaginatedSaveOptions::GetPageCount method


Gets or sets the number of pages to save.

```cpp
int32_t Aspose::Cells::PaginatedSaveOptions::GetPageCount()
```

## Remarks


Default is System.Int32.MaxValue which means all pages will be rendered.. 

## Examples


```cpp
Aspose::Cells::Startup();
//L'esempio seguente mostra come rendere un intervallo di pagine (3 e 4) in un file Microsoft Excel in PDF.
 //Apri un file Excel
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Stampa solo la Pagina 3 e la Pagina 4 nel PDF di output
//Indice della pagina iniziale (indice basato su 0)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Numero di pagine da stampare
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//Salva il file PDF
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
