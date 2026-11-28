---
title: "PageSetup.PaperWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfa yönelimi dikkate alınarak kağıdın genişliğini inç biriminde alır"
type: docs
url: /tr/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Sayfa yönü dikkate alınarak kağıdın genişliğini inç biriminde alır.

```csharp
public double PaperWidth { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı örnek veri ayarlayın
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // Çalışma sayfasının PageSetup'ına eriş
            PageSetup pageSetup = worksheet.PageSetup;
            
            // PaperWidth özelliğini göster (yalnızca okunabilir)
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // Kağıt boyutunu değiştirmek için, PaperSize özelliğini kullanın
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


