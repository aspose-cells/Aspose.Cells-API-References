---
title: "PageSetup.Orientation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfa baskı yönelimini temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Sayfa yazdırma yönünü temsil eder.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayfa yönelimini Yatay (Landscape) olarak ayarla
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // Etkiyi göstermek için bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


