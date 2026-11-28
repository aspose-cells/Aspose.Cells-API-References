---
title: "PageSetup.BlackAndWhite"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Belgenin öğelerinin siyah beyaz olarak yazdırılıp yazdırılmayacağını temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Belge öğelerinin siyah beyaz basılıp basılmayacağını temsil eder.

```csharp
public bool BlackAndWhite { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup nesnesini al
            PageSetup pageSetup = worksheet.PageSetup;

            // BlackAndWhite özelliğini true olarak ayarla
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // BlackAndWhite özelliğini false olarak değiştir
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


