---
title: "Worksheet.GridlineColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Izgara çizgi rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Kılavuz çizgilerinin rengini alır ve ayarlar.

```csharp
public Color GridlineColor { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Izgara çizgi rengini kırmızı olarak ayarla
            worksheet.GridlineColor = Color.Red;
            
            // Çalışma kitabını kaydedin
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


