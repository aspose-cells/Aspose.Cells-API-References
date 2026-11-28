---
title: "PageSetup.LeftMargin"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sol kenar boşluğunun boyutunu santimetre biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Sol kenar boşluğunun boyutunu santimetre biriminde temsil eder.

```csharp
public double LeftMargin { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bazı örnek veri ayarlayın
            sheet.Cells["A1"].PutValue("Left Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows how to set page margins");

            // Sol kenar boşluğunu (inç olarak) ayarla
            sheet.PageSetup.LeftMargin = 1.5;

            // Sol kenar boşluğu değerini konsola yazdır
            Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");

            // Kenar boşluğunu göstermek için PDF olarak kaydet
            string outputPath = "LeftMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("File saved with left margin: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


