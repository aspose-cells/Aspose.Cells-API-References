---
title: "GlowEffect.Transparency"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlowEffect özelliği. Parıltı efektinin şeffaflık derecesini alır ve ayarlar. 0.0 opakdan 1.0 şeffafa kadar"
type: docs
url: /tr/net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Parıltı etkisinin şeffaflık derecesini alır ve ayarlar. 0.0 (opak) ile 1.0 (şeffaf) arasında bir aralık.

```csharp
public double Transparency { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertyTransparencyDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            Shape shape = sheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 10, 0, 10, 200, 100);
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            
            CellsColor glowColor = shape.Glow.Color;
            glowColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            wb.Save("output/glow_transparency_demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


