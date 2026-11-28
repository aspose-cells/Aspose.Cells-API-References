---
title: "PageSetup.PaperSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Kağıdın boyutunu temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Kağıdın boyutunu temsil eder.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Kağıt boyutunu Envelope B6 olarak ayarla
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // Mevcut kağıt boyutunu yazdır
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


