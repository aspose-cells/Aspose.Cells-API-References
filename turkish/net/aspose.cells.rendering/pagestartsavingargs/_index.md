---
title: "PageStartSavingArgs sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PageStartSavingArgs sınıfı. Bir sayfanın kaydetme sürecinin başlangıcıyla ilgili bilgi"
type: docs
url: /tr/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Bir sayfanın kaydetme sürecinin başladığı hakkında bilgi.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Sayfanın çıktılanıp çıktılanmayacağını gösteren değeri alır veya ayarlar. Varsayılan değer doğrudur. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Toplam sayfa sayısı.([`PageSavingArgs`](../pagesavingargs/) üzerinden devralınmıştır.) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Geçerli sayfa indeksi, sıfır tabanlı.([`PageSavingArgs`](../pagesavingargs/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // İsteğe bağlı uygulama
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


