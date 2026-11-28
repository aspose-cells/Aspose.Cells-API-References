---
title: "PageSetup.PrintQuality"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Yazdırma kalitesini temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Yazdırma kalitesini temsil eder.

```csharp
public int PrintQuality { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yazdırma kalitesini 144 dpi olarak ayarla
            worksheet.PageSetup.PrintQuality = 144;
            
            // Mevcut yazdırma kalite ayarını yazdır
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


