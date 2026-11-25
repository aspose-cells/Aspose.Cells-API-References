---
title: "GlowEffect.Radius"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GlowEffect. Ottiene e imposta il raggio del bagliore in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/gloweffect/radius/
---
## GlowEffect.Radius property

Ottiene e imposta il raggio del bagliore, in unità di punti.

```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà GlowEffect.Size. Questa proprietà sarà rimossa 6 mesi dopo, a partire da settembre 2016. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

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

### Vedi anche

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


