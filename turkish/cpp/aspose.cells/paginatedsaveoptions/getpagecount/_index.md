---
title: Aspose::Cells::PaginatedSaveOptions::GetPageCount method
linktitle: GetPageCount
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PaginatedSaveOptions::GetPageCount method. Gets or sets the number of pages to save in C++.'
type: docs
weight: 2500
url: /tr/cpp/aspose.cells/paginatedsaveoptions/getpagecount/
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
//Aşağıdaki örnek, bir Microsoft Excel dosyasındaki (3 ve 4) sayfa aralığını PDF'ye nasıl render edeceğinizi gösterir.
 //Bir Excel dosyası aç
Workbook wb(u"Book1.xlsx");

PdfSaveOptions options;

//Çıktı PDF'sinde yalnızca Sayfa 3 ve Sayfa 4'ü yazdır
//Başlangıç sayfa indeksi (0 tabanlı indeks)
if (options.GetPageIndex() != 3)
{
    options.SetPageIndex(3);
}
//Yazdırılacak sayfa sayısı
if (options.GetPageCount() != 2)
{
    options.SetPageCount(2);
}

//PDF dosyasını kaydet
wb.Save(u"output.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PaginatedSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
