---
title: "GlowEffect.Size"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlowEffect. Obtiene y establece el radio del resplandor en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Obtiene y establece el radio del resplandor, en unidades de puntos.

```csharp
public double Size { get; set; }
```

### Ejemplos

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
            
            // Establecer propiedades del efecto de resplandor
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            shape.Glow.Color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


