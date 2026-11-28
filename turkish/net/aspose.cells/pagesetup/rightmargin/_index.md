---
title: "PageSetup.RightMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sağ kenar boşluğunun boyutunu santimetre biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/rightmargin/
---
## PageSetup.RightMargin property

Sağ kenar boşluğunun boyutunu, santimetre biriminde temsil eder.

```csharp
public double RightMargin { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı sağ kenar boşlukları ayarla ve etkiyi göstermek için kaydet
            worksheet.PageSetup.RightMargin = 0;
            workbook.Save("RightMargin_0.xlsx");

            worksheet.PageSetup.RightMargin = 1.0;
            workbook.Save("RightMargin_1.xlsx");

            worksheet.PageSetup.RightMargin = 2.5;
            workbook.Save("RightMargin_2.5.xlsx");

            // Mevcut sağ kenar boşluğu değerini yazdır
            Console.WriteLine("Current Right Margin: " + worksheet.PageSetup.RightMargin);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


