---
title: "GlowEffect.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlowEffect. Obtiene el color del efecto de resplandor"
type: docs
url: /es/net/aspose.cells.drawing/gloweffect/color/
---
## GlowEffect.Color property

Obtiene el color del efecto de resplandor.

```csharp
public CellsColor Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 10, 10, 100, 100, 100, 100);
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            
            CellsColor glowColor = shape.Glow.Color;
            glowColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


