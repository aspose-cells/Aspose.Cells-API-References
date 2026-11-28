---
title: "PageSetup.TopMarginInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Üst kenar boşluğunun inç birimindeki boyutunu temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Üst kenar boşluğunun boyutunu, inç biriminde temsil eder.

```csharp
public double TopMarginInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Üst kenar boşluğunu 1.5 inç olarak ayarla
            sheet.PageSetup.TopMarginInch = 1.5;

            // Üst kenar boşluğu değerini al ve yazdır
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


