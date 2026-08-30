---
title: Aspose::Cells::PaginatedSaveOptions::SetPageCount method
linktitle: SetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2400
url: /fr/cpp/aspose.cells/paginatedsaveoptions/setpagecount/
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
//L’exemple suivant montre comment rendre une plage de pages (3 et 4) d’un fichier Microsoft Excel en PDF.
 //Ouvrez un fichier Excel
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Imprimez uniquement la page 3 et la page 4 dans le PDF de sortie
//Indice de page de départ (indice basé sur 0)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Nombre de pages à imprimer
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//Enregistrez le fichier PDF
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
