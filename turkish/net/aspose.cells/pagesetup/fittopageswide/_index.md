---
title: "PageSetup.FitToPagesWide"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Çalışma sayfasının yazdırıldığında kaç sayfa genişliğine ölçekleneceğini temsil eder. Varsayılan değer 1'dir"
type: docs
url: /tr/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Çalışma sayfasının yazdırıldığında ölçekleneceği sayfa genişliğini temsil eder. Varsayılan değer 1'dir.

```csharp
public int FitToPagesWide { get; set; }
```

### Açıklamalar

Tüm sütunları tek bir sayfaya sığdırmak istiyorsanız FitToPagesTall değerini sıfır olarak ayarlamanız gerekir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // Sayfa ayarı özelliklerini ayarla
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // Çalışma kitabını kaydedin
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


