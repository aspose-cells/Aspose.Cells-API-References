---
title: "PageSetup.PrintArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Yazdırılacak aralığı temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Yazdırılacak aralığı temsil eder.

```csharp
public string PrintArea { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(3);
            
            // Yazdırma alanını A1:B3 olarak ayarla
            worksheet.PageSetup.PrintArea = "A1:B3";
            
            // Yalnızca yazdırma alanı ile kaydet
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportPrintAreaOnly = true
            };
            
            workbook.Save("PrintAreaDemo.html", options);
            
            Console.WriteLine("Print area demo created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


