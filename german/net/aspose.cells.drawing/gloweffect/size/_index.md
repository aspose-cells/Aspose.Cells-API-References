---
title: "GlowEffect.Size"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlowEffect-Eigenschaft. Gibt den Radius des Leuchteffekts zurück und legt ihn fest, gemessen in Punkt-Einheiten"
type: docs
url: /de/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Liest und setzt den Radius des Leuchteffekts in Punkten.

```csharp
public double Size { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 10, 10, 200, 100, 200, 100);
            
            // Glow-Effekt-Eigenschaften festlegen
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


