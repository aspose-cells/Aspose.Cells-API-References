---
title: "PageSetup.HeaderMarginInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfanın üstünden başlığa kadar olan mesafeyi inç biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi inç biriminde temsil eder.

```csharp
public double HeaderMarginInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginInchDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına ve onun PageSetup'ına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Başlık kenar boşluğunu inç cinsinden ayarla
            pageSetup.HeaderMarginInch = 0.5;
            
            // Gösterim için diğer kenar boşluklarını ayarla
            pageSetup.FooterMarginInch = 0.25;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetupMargins.xlsx");

            // Başlık kenar boşluğu değerini göster
            Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


