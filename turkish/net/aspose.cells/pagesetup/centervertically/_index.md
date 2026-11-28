---
title: "PageSetup.CenterVertically"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfanın dikey olarak ortalanmış şekilde yazdırılıp yazdırılmayacağını temsil eder."
type: docs
url: /tr/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Sayfanın dikey olarak ortalanmış şekilde basılıp basılmayacağını temsil eder.

```csharp
public bool CenterVertically { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // PageSetup'a eriş ve CenterVertically'i ayarla
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // Etkiyi görselleştirmek için bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


