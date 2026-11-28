---
title: "ImageOrPrintOptions.PrintingPage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Hangi sayfaların yazdırılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/printingpage/
---
## ImageOrPrintOptions.PrintingPage property

Hangi sayfaların yazdırılmayacağını gösterir.

```csharp
public PrintingPageType PrintingPage { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintingPageDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["A2"].PutValue("Non-Blank Cell");
            worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
            
            // Görüntü/baskı seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.IgnoreBlank;
            
            // Çalışma kitabını seçeneklerle oluştur
            WorkbookRender render = new WorkbookRender(workbook, options);
            
            // Sayfa sayısını çıktıla (boş sayfalar yok sayılacak)
            Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
            
            // Varsayılan davranışa değiştir (tüm sayfaları dahil et)
            options.PrintingPage = PrintingPageType.Default;
            render = new WorkbookRender(workbook, options);
            Console.WriteLine("Page count with Default: " + render.PageCount);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


