---
title: "ScrollBar.Shadow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScrollBar özelliği. Şeklin 3D gölgelendirmeye sahip olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/scrollbar/shadow/
---
## ScrollBar.Shadow property

Şeklin 3B gölgelendirmeye sahip olup olmadığını gösterir.

```csharp
public bool Shadow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyShadowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yatay bir kaydırma çubuğu ekle
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
            
            // Kaydırma çubuğu özelliklerini ayarlayın
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;
            scrollBar.CurrentValue = 50;
            scrollBar.IsHorizontal = true;
            
            // Shadow özelliğini göster
            scrollBar.Shadow = true; // Enable 3D shadow effect
            
            // Karşılaştırma için başka bir kaydırma çubuğu oluştur
            ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
            scrollBar2.Shadow = false; // No shadow
            
            // Çalışma kitabını kaydedin
            workbook.Save("ScrollBarShadowDemo.xlsx");
            
            Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


