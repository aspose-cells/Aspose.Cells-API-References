---
title: "PageSetup.PrintDraft"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Sayfanın grafikler olmadan yazdırılıp yazdırılmayacağını temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Sayfanın grafikler olmadan yazdırılıp yazdırılmayacağını temsil eder.

```csharp
public bool PrintDraft { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PageSetup nesnesine erişin
            PageSetup pageSetup = worksheet.PageSetup;

            // PrintDraft özelliğini true olarak ayarla
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // PrintDraft özelliğini false olarak değiştir
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // Çalışma kitabını kaydedin
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


