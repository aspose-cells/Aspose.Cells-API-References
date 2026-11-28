---
title: "PageSetup.IsHFDiffOddEven"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. True, tek sayfaların üstbilgi/altbilgisinin tek sayfalarla farklı olduğunu ifade eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

Doğru, tek sayfaların üst bilgi/alt bilgisinin diğer tek sayfalardan farklı olduğunu gösterir.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // PageSetup'a eriş
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Tek ve çift sayfalar için farklı üstbilgi/altbilgi etkinleştir
            pageSetup.IsHFDiffOddEven = true;
            
            // Tek ve çift sayfalar için farklı altbilgiler ayarla
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // Kaydedilen dosyayı yükleyerek ayarları doğrula
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


