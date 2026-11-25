---
title: "GlowEffect.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GlowEffect. Ottiene e imposta il grado di trasparenza dell'effetto di bagliore. Intervallo da 0,0 opaco a 1,0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Ottiene e imposta il grado di trasparenza dell'effetto bagliore. Intervallo da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

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

### Vedi anche

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


