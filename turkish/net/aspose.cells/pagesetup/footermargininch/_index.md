---
title: "PageSetup.FooterMarginInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfanın alt kısmı ile altbilgi arasındaki mesafeyi inç biriminde temsil eder."
type: docs
url: /tr/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi inç biriminde temsil eder.

```csharp
public double FooterMarginInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına ve onun PageSetup'ına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Altbilgi kenar boşluğunu inç cinsinden ayarla
            pageSetup.FooterMarginInch = 0.5;
            
            // Gösterim için diğer kenar boşluklarını ayarla
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageSetupMargins.xlsx");
            
            // Onayı yazdır
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


