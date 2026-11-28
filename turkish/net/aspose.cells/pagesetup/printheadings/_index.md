---
title: "PageSetup.PrintHeadings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Bu sayfada satır ve sütun başlıklarının yazdırılıp yazdırılmayacağını temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/printheadings/
---
## PageSetup.PrintHeadings property

Satır ve sütun başlıklarının bu sayfada basılıp basılmayacağını temsil eder.

```csharp
public bool PrintHeadings { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintHeadingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Başlıklarla birlikte bazı örnek verileri ayarla
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Başlıkların yazdırılmasını etkinleştir
            worksheet.PageSetup.PrintHeadings = true;
            worksheet.PageSetup.PrintArea = "A1:B3";

            // Etkiyi göstermek için HTML olarak kaydet
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportActiveWorksheetOnly = true,
                ExportPrintAreaOnly = true,
                ExportGridLines = true,
                ExportHeadings = true
            };

            workbook.Save("PrintHeadingsDemo.html", saveOptions);

            Console.WriteLine("Worksheet saved with PrintHeadings enabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


