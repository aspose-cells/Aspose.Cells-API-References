---
title: "GlowEffect.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlowEffect-egenskap. Hämtar och anger graden av transparens för glow-effekten. Omfång från 0,0 ogenomskinlig till 1,0 klar"
type: docs
url: /sv/net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Hämtar och anger graden av transparens för glödeffekten. Omfång från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

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

### Se även

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


