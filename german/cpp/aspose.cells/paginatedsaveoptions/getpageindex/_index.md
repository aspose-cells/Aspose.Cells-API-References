---
title: Aspose::Cells::PaginatedSaveOptions::GetPageIndex method
linktitle: GetPageIndex
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetPageIndex method. Gets or sets the 0-based index of the first page to save in C++.'
type: docs
weight: 2300
url: /de/cpp/aspose.cells/paginatedsaveoptions/getpageindex/
---
## PaginatedSaveOptions::GetPageIndex method


Gets or sets the 0-based index of the first page to save.

```cpp
int32_t Aspose::Cells::PaginatedSaveOptions::GetPageIndex()
```

## Remarks


Default is 0. 

## Examples


```cpp
Aspose::Cells::Startup();
//Das folgende Beispiel zeigt, wie man einen Bereich von Seiten (3 und 4) in einer Microsoft Excel-Datei zu PDF rendert.
 //Öffne eine Excel-Datei
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Drucke nur Seite 3 und Seite 4 im Ausgabe-PDF
//Startseitenindex (0-basierter Index)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Anzahl der zu druckenden Seiten
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//Speichere die PDF-Datei
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
