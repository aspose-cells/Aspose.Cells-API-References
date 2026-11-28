---
title: "PageSetup.PrintGridlines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Hücre ızgaralarının sayfada yazdırılıp yazdırılmayacağını temsil eder."
type: docs
url: /tr/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Hücre ızgara çizgilerinin sayfada basılıp basılmayacağını temsil eder.

```csharp
public bool PrintGridlines { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreye örnek veri koy
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // PrintGridlines özelliğini değiştir
            worksheet.PageSetup.PrintGridlines = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


