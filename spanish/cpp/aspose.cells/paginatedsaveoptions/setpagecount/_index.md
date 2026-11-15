---
title: Aspose::Cells::PaginatedSaveOptions::SetPageCount method
linktitle: SetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2400
url: /es/cpp/aspose.cells/paginatedsaveoptions/setpagecount/
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
//El siguiente ejemplo muestra cómo renderizar un rango de páginas (3 y 4) en un archivo Microsoft Excel a PDF.
 //Abrir un archivo Excel
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Imprimir solo la página 3 y la página 4 en el PDF de salida
//Índice de página inicial (índice basado en 0)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Número de páginas a imprimir
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//Guardar el archivo PDF
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
