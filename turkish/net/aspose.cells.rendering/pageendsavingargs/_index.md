---
title: "Sınıf PageEndSavingArgs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PageEndSavingArgs sınıfı. Bir sayfanın kaydetme sürecinin sonu hakkında bilgi"
type: docs
url: /tr/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

Bir sayfa için bilgi, kaydetme sürecini sonlandırır.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Daha fazla sayfanın çıktısı olup olmadığını gösteren bir değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Toplam sayfa sayısı.([`PageSavingArgs`](../pagesavingargs/) üzerinden devralınmıştır.) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Geçerli sayfa indeksi, sıfır tabanlı.([`PageSavingArgs`](../pagesavingargs/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // PdfSaveOptions sınıfının bir örneğini oluşturun
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // PageEndSaving geri çağrısını ayarla
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // Çalışma kitabını geri çağrı ile kaydet
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Bu demo için uygulama gerekmez
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


