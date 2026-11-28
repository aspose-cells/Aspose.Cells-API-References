---
title: "ScrollBar.Min"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScrollBar özelliği. Bir kaydırma çubuğu veya döndürme aralığının minimum değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

Kaydırma çubuğu veya döndürme düğmesi aralığının minimum değerini alır veya ayarlar.

```csharp
public int Min { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir kaydırma çubuğu ekleyin
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Kaydırma çubuğu özelliklerini ayarlayın
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Min özelliği değerini gösterin
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // Çalışma kitabını kaydedin
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


