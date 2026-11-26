---
title: "GlowEffect.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlowEffect. Obtiene y establece el grado de transparencia del efecto de resplandor. Rango de 0,0 opaco a 1,0 claro"
type: docs
url: /es/net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Obtiene y establece el grado de transparencia del efecto de resplandor. Rango de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

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

### Ver también

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


