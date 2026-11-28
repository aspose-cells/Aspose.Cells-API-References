---
title: "PageSetup.CustomPaperSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Özel kağıt boyutunu inç biriminde ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Özel kağıt boyutunu, inç biriminde ayarlar.

```csharp
public void CustomPaperSize(double width, double height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| genişlik | Double | Kağıdın genişliği. |
| yükseklik | Double | Kağıdın yüksekliği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel kağıt boyutunu ayarla (genişlik: 1.5 inç, yükseklik: 1.5 inç)
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // Etkiyi göstermek için çalışma kitabını kaydedin
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


