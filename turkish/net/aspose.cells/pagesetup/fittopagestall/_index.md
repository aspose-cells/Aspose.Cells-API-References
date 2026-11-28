---
title: "PageSetup.FitToPagesTall"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Çalışma sayfasının yazdırıldığında kaç sayfa yüksekliğine ölçekleneceğini temsil eder. Varsayılan değer 1'dir."
type: docs
url: /tr/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

Çalışma sayfasının yazdırıldığında ölçekleneceği sayfa yüksekliğini temsil eder. Varsayılan değer 1'dir.

```csharp
public int FitToPagesTall { get; set; }
```

### Açıklamalar

Tüm satırları tek sayfaya sığdırmak istiyorsanız FitToPagesWide'ı sıfır olarak ayarlamanız gerekir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayfanın birden fazla sayfaya yayılması için örnek veri ekleyin
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // PageSetup nesnesini al
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Yazdırma alanını ayarla
            pageSetup.PrintArea = "A1:J100";
            
            // FitToPagesTall özelliğini tüm satırları tek sayfaya sığacak şekilde ayarla
            pageSetup.FitToPagesTall = 1;
            
            // FitToPagesWide özelliğini tüm sütunları tek sayfaya sığacak şekilde ayarla
            pageSetup.FitToPagesWide = 1;
            
            // Kağıt boyutunu ayarla
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Izgara çizgilerini yazdır
            pageSetup.PrintGridlines = true;

            // Renderleme seçeneklerini oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Sayfa oluşturucusunu oluştur
            SheetRender render = new SheetRender(worksheet, options);
            
            // Sayfa ölçeğini çıktı olarak ver
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


