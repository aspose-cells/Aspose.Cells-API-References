---
title: "GlowEffect.Radius"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlowEffect. Obtiene y establece el radio del resplandor en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/gloweffect/radius/
---
## GlowEffect.Radius property

Obtiene y establece el radio del resplandor, en unidades de puntos.

```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad GlowEffect.Size. Esta propiedad será eliminada 6 meses después desde septiembre de 2016. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GlowEffectPropertyRadiusDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
            arcShape.Placement = PlacementType.FreeFloating;
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = System.Drawing.Color.Blue;

            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = System.Drawing.Color.Yellow;
            glowEffect.Radius = 15.0; // Demonstrating Radius property
            glowEffect.Transparency = 0.3;

            workbook.Save("GlowEffectRadiusDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


