---
title: "ScrollBar.Max"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScrollBar özelliği. Kaydırma çubuğu veya döndürme düğmesi aralığının maksimum değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/scrollbar/max/
---
## ScrollBar.Max property

Kaydırma çubuğu veya döndürme düğmesi aralığının maksimum değerini alır veya ayarlar.

```csharp
public int Max { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMaxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir kaydırma çubuğu ekleyin
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Kaydırma çubuğu özelliklerini ayarlayın
            scrollBar.Min = 0;
            scrollBar.Max = 100; // Demonstrating Max property usage
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 10;

            // Çalışma kitabını kaydedin
            workbook.Save("ScrollBarMaxDemo.xlsx");

            // Bilgiyi göster
            Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
            Console.WriteLine("File saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


