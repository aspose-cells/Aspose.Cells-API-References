---
title: "PageSetup.IsAutomaticPaperSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Kağıt boyutunun otomatik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

Kağıt boyutunun otomatik olup olmadığını gösterir.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutomaticPaperSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayfa ayarına eriş
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Otomatik kağıt boyutu değerini al
            Console.WriteLine("Automatic Paper Size: " + pageSetup.IsAutomaticPaperSize);
            
            // Farklı ayarlarla başka bir çalışma kitabı oluştur
            Workbook workbook2 = new Workbook("example.xlsx");
            PageSetup pageSetup2 = workbook2.Worksheets[0].PageSetup;
            Console.WriteLine("Automatic Paper Size from file: " + pageSetup2.IsAutomaticPaperSize);
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


