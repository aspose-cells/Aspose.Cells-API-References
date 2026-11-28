---
title: "PageSetup.HeaderMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfanın üstünden üst bilgiye olan mesafeyi santimetre biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

Sayfanın üst kısmı ile üst bilgi arasındaki mesafeyi santimetre biriminde temsil eder.

```csharp
public double HeaderMargin { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup'a eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // Üst bilgi kenar boşluğunu santimetre olarak ayarla
            pageSetup.HeaderMargin = 1.5;

            // Üst bilgi kenar boşluğunun ayarlandığını doğrula
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // Çalışma kitabını kaydedin
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


