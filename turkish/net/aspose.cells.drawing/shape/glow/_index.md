---
title: "Shape.Glow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Grafik öğesi veya şekil için parlama etkisini belirten bir GlowEffect nesnesini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

[`GlowEffect`](../../gloweffect/) nesnesini temsil eder ve grafik öğesi veya şekil için parlama etkisini belirtir.

```csharp
public GlowEffect Glow { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGlowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Parlama etkisine eriş
            GlowEffect glow = shape.Glow;

            // Parlama özelliklerini ayarla
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


