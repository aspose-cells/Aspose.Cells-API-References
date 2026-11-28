---
title: "PageSetup.Zoom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Yüzde olarak ölçekleme faktörünü temsil eder. 10 ile 400 arasında olmalıdır."
type: docs
url: /tr/net/aspose.cells/pagesetup/zoom/
---
## PageSetup.Zoom property

Yüzde cinsinden ölçek faktörünü temsil eder. 10 ile 400 arasında olmalıdır.

```csharp
public int Zoom { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyZoomDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yakınlaştırma seviyesini %150'ye ayarla
            worksheet.PageSetup.Zoom = 150;
            
            // Mevcut yakınlaştırma seviyesini yazdır
            Console.WriteLine("Current Zoom Level: " + worksheet.PageSetup.Zoom);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


