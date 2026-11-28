---
title: "PageSetup.SetFitToPages"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Çalışma sayfasının yazdırıldığında ölçekleneceği sayfa sayısını ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Çalışma sayfasının yazdırıldığında ölçekleneceği sayfa sayısını ayarlar.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| geniş | Int32 | Sayfa genişliği. |
| uzun | Int32 | Sayfa uzunluğunda. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasının PageSetup'ına eriş
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Sayfalara sığdırma ayarlarını ayarla
            setup.SetFitToPages(2, 3);
            
            // Ayarları doğrula ve çıktı al
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
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


