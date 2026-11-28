---
title: "PageSetup.FooterMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi santimetre biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Sayfanın alt kısmı ile alt bilgi arasındaki mesafeyi santimetre biriminde temsil eder.

```csharp
public double FooterMargin { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup'a eriş
            PageSetup pageSetup = worksheet.PageSetup;

            // Alt bilgi kenar boşluğunu santimetre olarak ayarlayın
            pageSetup.FooterMargin = 1.5;

            // Etkiyi görmek için biraz içerik ekleyin
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // Kenar boşluğunu görünür kılmak için alt bilgi metnini ayarlayın
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // Çalışma kitabını kaydedin
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


