---
title: "PageSetup.IsHFDiffFirst"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. True, ilk sayfanın üstbilgi/altbilgisinin diğer sayfalardan farklı olduğu anlamına gelir"
type: docs
url: /tr/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

Doğru, ilk sayfanın üst bilgi/alt bilgisinin diğer sayfalardan farklı olduğunu ifade eder.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // PageSetup'a eriş
            PageSetup pageSetup = worksheet.PageSetup;
            
            // İlk sayfa için farklı başlık/altbilgiler ayarla
            pageSetup.IsHFDiffFirst = true;
            
            // Üstbilgi/altbilgileri ayarla
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // Ayarları doğrulamak için çalışma kitabını yeniden yükle
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // Doğrulamayı çıktı olarak ver
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


