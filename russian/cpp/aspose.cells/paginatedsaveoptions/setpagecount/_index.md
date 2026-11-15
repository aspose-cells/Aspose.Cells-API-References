---
title: Aspose::Cells::PaginatedSaveOptions::SetPageCount method
linktitle: SetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::SetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2400
url: /ru/cpp/aspose.cells/paginatedsaveoptions/setpagecount/
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
//Следующий пример показывает, как отобразить диапазон страниц (3 и 4) из файла Microsoft Excel в PDF.
 //Открыть файл Excel
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Печатать только страницу 3 и страницу 4 в результирующем PDF
//Начальный индекс страницы (нумерация с нуля)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Количество страниц для печати
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//Сохранить PDF‑файл
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
