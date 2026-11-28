---
title: "PageSetup.BottomMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Alt kenar boşluğunun santimetre birimindeki boyutunu temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Alt kenar boşluğunun boyutunu santimetre biriminde temsil eder.

```csharp
public double BottomMargin { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı örnek veri ayarlayın
            worksheet.Cells["A1"].PutValue("Sample Text for Margin Demonstration");
            
            // Alt kenar boşluğu ile sayfa ayarını yapılandırın
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.BottomMargin = 0.5; // 0.5 inch bottom margin
            pageSetup.TopMargin = 1.0;    // 1 inch top margin
            pageSetup.LeftMargin = 0.75;  // 0.75 inch left margin
            pageSetup.RightMargin = 0.75; // 0.75 inch right margin

            // Kenar boşluklarını göstermek için PDF olarak kaydedin
            workbook.Save("PageMarginsDemo.pdf", SaveFormat.Pdf);

            Console.WriteLine("Document with bottom margin of 0.5 inches created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


