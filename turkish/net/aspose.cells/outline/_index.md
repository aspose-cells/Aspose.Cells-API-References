---
title: "Sınıf Outline"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Outline sınıfı. Bir çalışma sayfasındaki anahatı temsil eder"
type: docs
url: /tr/net/aspose.cells/outline/
---
## Outline class

Çalışma sayfasındaki bir taslağı temsil eder.

```csharp
public class Outline
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [SummaryColumnRight](../../aspose.cells/outline/summarycolumnright/) { get; set; } | Anahattaki özet sütununun detay sütunlarının sağında konumlandırılıp konumlandırılmayacağını gösterir. |
| [SummaryRowBelow](../../aspose.cells/outline/summaryrowbelow/) { get; set; } | Anahattaki özet satırının detay satırlarının altında konumlandırılıp konumlandırılmayacağını gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OutlineDemo
    {
        public static void OutlineExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabındaki ilk çalışma sayfasına erişin
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasının anahattına eriş
            Outline outline = worksheet.Outline;
            
            // Anahattın özelliklerini ayarla
            outline.SummaryRowBelow = true; // Indicates if the summary row will be positioned below the detail rows
            outline.SummaryColumnRight = true; // Indicates if the summary column will be positioned to the right of the detail columns
            
            // Çalışma kitabını kaydedin
            workbook.Save("OutlineExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


