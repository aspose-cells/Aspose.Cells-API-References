---
title: "PageSetup.BottomMarginInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Alt kenar boşluğunun inç cinsinden boyutunu temsil eder."
type: docs
url: /tr/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Alt kenar boşluğunun boyutunu inç biriminde temsil eder.

```csharp
public double BottomMarginInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasının PageSetup'ına eriş
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Çeşitli kenar boşluklarını inç cinsinden ayarla
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageMarginsDemo.xlsx");
            
            // Onayı göster
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


