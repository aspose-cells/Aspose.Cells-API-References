---
title: "GlowEffect.Size"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GlowEffect. Ottiene e imposta il raggio del bagliore in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Ottiene e imposta il raggio del bagliore, in unità di punti.

```csharp
public double Size { get; set; }
```

### Esempi

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
            
            // Imposta le proprietà dell'effetto bagliore
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


