---
title: "PageSetup.PrintTitleRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Her sayfanın üst kısmında tekrarlanacak hücreleri içeren satırları temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

Her sayfanın üst kısmında tekrarlanacak hücreleri içeren satırları temsil eder.

```csharp
public string PrintTitleRows { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı örnek veri ayarlayın
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // Sayfa ayarına eriş
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Yazdırma başlık satırlarını ayarla (ilk satır her basılan sayfada tekrar eder)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // Çalışma kitabını kaydedin
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


