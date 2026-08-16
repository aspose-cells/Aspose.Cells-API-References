---
title: Aspose::Cells::PaginatedSaveOptions::SetPageCount method
linktitle: SetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2400
url: /de/cpp/aspose.cells/paginatedsaveoptions/setpagecount/
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
