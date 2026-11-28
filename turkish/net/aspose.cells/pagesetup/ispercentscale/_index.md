---
title: "PageSetup.IsPercentScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Bu özellik False ise FitToPagesWide ve FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

Bu özellik Yanlış ise, FitToPagesWide ve FitToPagesTall özellikleri çalışma sayfasının nasıl ölçeklendirileceğini kontrol eder.

```csharp
public bool IsPercentScale { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup'a eriş ve ölçeklemeyi %80'e (yüzde ölçeği) ayarla
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // IsPercentScale'i göstermek için ayarları çıktı olarak ver
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


