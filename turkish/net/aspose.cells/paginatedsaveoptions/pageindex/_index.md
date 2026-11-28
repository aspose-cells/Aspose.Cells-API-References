---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Kaydedilecek ilk sayfanın 0 tabanlı indeksini alır veya ayarlar.

```csharp
public int PageIndex { get; set; }
```

### Açıklamalar

Varsayılan 0'dır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Birden fazla sayfada örnek veri ekleyin
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // PDF kaydetme seçeneklerini ayarlayın
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Sayfaları 3-4 (0 tabanlı indeks) yazdırmak için ayarlayın
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // Seçili sayfalarla PDF'yi kaydedin
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


