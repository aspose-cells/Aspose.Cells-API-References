---
title: "GlowEffect.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlowEffect-Eigenschaft. Gibt den Transparenzgrad des Leuchteffekts zurück und legt ihn fest. Bereich von 0,0 (undurchsichtig) bis 1,0 (transparent)"
type: docs
url: /de/net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Liest und setzt den Transparenzgrad des Leuchteffekts. Bereich von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

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

### Siehe auch

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


