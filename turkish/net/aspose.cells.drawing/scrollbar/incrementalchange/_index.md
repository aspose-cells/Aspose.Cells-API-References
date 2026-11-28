---
title: "ScrollBar.IncrementalChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScrollBar özelliği. Kaydırma çubuğu veya döndürme düğmesinin bir satır kaydırma ile artırıldığı miktarı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

Kaydırma çubuğu veya döndürme düğmesinin bir satır kaydırma ile artırıldığı miktarı alır veya ayarlar.

```csharp
public int IncrementalChange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir kaydırma çubuğu ekleyin
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Kaydırma çubuğu özelliklerini ayarlayın
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // Kaydırma çubuğu özelliklerini göster
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // Artımlı değişikliği değiştir
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

            // Çalışma kitabını kaydedin
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


