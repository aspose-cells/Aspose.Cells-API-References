---
title: "PaginatedSaveOptions.PageCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Kaydedilecek sayfa sayısını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

Kaydedilecek sayfa sayısını alır veya ayarlar.

```csharp
public int PageCount { get; set; }
```

### Açıklamalar

Varsayılan System.Int32.MaxValue'dir, bu da tüm sayfaların render edileceği anlamına gelir..

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Bir Excel dosyası açın
            Workbook wb = new Workbook("Book1.xlsx");
            
            // PDF kaydetme seçeneklerini başlatın
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Sayfa 4'ten (0 tabanlı indeks 3) başlayarak yalnızca 2 sayfa yazdıracak şekilde ayarlayın
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // PDF dosyasını kaydedin
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


