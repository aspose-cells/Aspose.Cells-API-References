---
title: "PageEndSavingArgs.HasMorePages"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageEndSavingArgs özelliği. Daha fazla sayfanın çıktıya alınacağını gösteren bir değeri alır veya ayarlar. Varsayılan değer true'dur."
type: docs
url: /tr/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

Daha fazla sayfanın çıktısı olup olmadığını gösteren bir değeri alır veya ayarlar. Varsayılan değer doğrudur.

```csharp
public bool HasMorePages { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageEndSavingArgsPropertyHasMorePagesDemo
    {
        public static void Run()
        {
            // Verilerin birden çok sayfaya yayıldığı bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // Özel sayfa işleme ile PDF kaydetme seçenekleri oluştur
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // Çalışma kitabını sayfa sınırlamasıyla kaydet
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Bu gösterimde kullanılmaz
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Mevcut özellik değerini oku
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // İlk sayfadan sonra özelliği değiştir
            if (pageCount == 0)
            {
                args.HasMorePages = false;
                Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
            }

            pageCount++;
        }
    }
}
```

### Ayrıca Bakınız

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


