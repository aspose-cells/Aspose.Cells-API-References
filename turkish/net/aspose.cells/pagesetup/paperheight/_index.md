---
title: "PageSetup.PaperHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Kağıdın yüksekliğini inç biriminde alır, sayfa yönelimi dikkate alınır."
type: docs
url: /tr/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

Sayfa yönü dikkate alınarak kağıdın yüksekliğini inç biriminde alır.

```csharp
public double PaperHeight { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir hücreye bazı veriler ayarla
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // PageSetup nesnesini al
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Varsayılan kağıt yüksekliğini göster (inç olarak)
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight yalnızca okunabilir, bu yüzden farklı kağıt boyutlarını almayı gösteriyoruz
            // kağıt boyutu tipini Letter (8.5x11 inç) olarak değiştirerek
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Değişikliği doğrulayın
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


