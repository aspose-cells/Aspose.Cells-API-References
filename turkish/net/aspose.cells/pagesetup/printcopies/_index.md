---
title: "PageSetup.PrintCopies"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Yazdırılacak kopya sayısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Yazdırılacak kopya sayısını alır ve ayarlar.

```csharp
public int PrintCopies { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yazdırma kopya sayısını 3 olarak ayarla
            worksheet.PageSetup.PrintCopies = 3;
            
            // Mevcut yazdırma kopya ayarını göster
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


