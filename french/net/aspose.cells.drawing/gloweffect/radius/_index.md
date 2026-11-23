---
title: "GlowEffect.Radius"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GlowEffect. Obtient et définit le rayon de la lueur en unités de points"
type: docs
url: /fr/net/aspose.cells.drawing/gloweffect/radius/
---
## GlowEffect.Radius property

Obtient et définit le rayon de la lueur, en unité de points.

```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété GlowEffect.Size. Cette propriété sera supprimée 6 mois plus tard à compter de septembre 2016. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

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

### Voir aussi

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


