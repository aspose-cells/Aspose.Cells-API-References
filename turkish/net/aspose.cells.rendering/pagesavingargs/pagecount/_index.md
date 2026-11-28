---
title: "PageSavingArgs.PageCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSavingArgs özelliği. Toplam sayfa sayısı"
type: docs
url: /tr/net/aspose.cells.rendering/pagesavingargs/pagecount/
---
## PageSavingArgs.PageCount property

Toplam sayfa sayısı.

```csharp
public int PageCount { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingArgsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve test verileri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Birden fazla sayfa oluşturmak için yoğun içerik ekleyin
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Sayfa ayarlarını belirleyerek sayfalama kontrolü yapın
            worksheet.PageSetup.PrintArea = "A1:A50";
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Sayfa kaydetme geri aramasıyla PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new PageSavingCallback();

            // Sayfalama tetiklemek için PDF olarak kaydedin
            workbook.Save("PageSavingDemo.pdf", options);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Olay argümanlarından PageCount değerine erişin
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Uygulama gerekmez
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


