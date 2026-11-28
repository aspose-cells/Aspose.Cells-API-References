---
title: "PageSetup.LeftMarginInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sol kenar boşluğunun boyutunu inç biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

Sol kenar boşluğunun boyutunu inç biriminde temsil eder.

```csharp
public double LeftMarginInch { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup'a eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // Sol kenar boşluğunu inç cinsinden ayarlayın (0.39 inç ≈ 1 cm)
            pageSetup.LeftMarginInch = 0.39;

            // Kenar boşluğunu göstermek için biraz veri ekleyin
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // Çalışma kitabını kaydedin
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


