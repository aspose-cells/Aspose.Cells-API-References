---
title: "PageSavingArgs.PageIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSavingArgs özelliği. Geçerli sayfa indeksi sıfır tabanlı"
type: docs
url: /tr/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

Geçerli sayfa indeksi, sıfır tabanlı.

```csharp
public int PageIndex { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSavingArgsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı veriler ekle
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Sayfa kaydetme geri aramasını ayarlayın
            options.PageSavingCallback = new PageSavingCallback();

            // Çalışma kitabını PDF olarak kaydedin - bu, her sayfa için geri aramayı tetikleyecektir
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // PageIndex özelliğinin kullanımını gösterin
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Bu örnekte kullanılmaz
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


