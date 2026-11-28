---
title: "Sınıf PageSavingArgs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PageSavingArgs sınıfı. Bir sayfa kaydetme süreci için bilgi"
type: docs
url: /tr/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

Bir sayfa kaydetme işlemi için bilgi.

```csharp
public class PageSavingArgs
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Toplam sayfa sayısı. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Geçerli sayfa indeksi, sıfır tabanlı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassPageSavingArgsDemo
    {
        public static void Run()
        {
            // Birden fazla sayfa için genişletilmiş veriyle yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Render edildiğinde birden fazla sayfa üretmek için çalışma sayfasını doldur
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // Sayfa kaydetme geri çağrımıyla PDF kaydetme seçeneklerini yapılandır
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // Çalışma kitabını sayfalama ile PDF formatında kaydet
            workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
                
                if (args.PageIndex == 0)
                {
                    Console.WriteLine("Processing cover page...");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // İsteğe bağlı: Buraya sayfa sonu işleme ekleyin
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


