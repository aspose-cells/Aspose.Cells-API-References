---
title: "PageSetup.RightMarginInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sağ kenar boşluğunun inç birimindeki boyutunu temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/rightmargininch/
---
## PageSetup.RightMarginInch property

Sağ kenar boşluğunun boyutunu, inç biriminde temsil eder.

```csharp
public double RightMarginInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup'a erişin ve RightMarginInch'i ayarlayın
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.RightMarginInch = 0.75; // Set right margin to 0.75 inches

            // Etkiyi görmek için bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Right Margin Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["B" + i].PutValue("Sample Data " + i);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RightMarginInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


