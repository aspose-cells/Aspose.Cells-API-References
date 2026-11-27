---
title: "GlowEffect.Radius"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlowEffect-egenskap. Hämtar och anger radien för glow i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/gloweffect/radius/
---
## GlowEffect.Radius property

Hämtar och anger glödens radie i enheter av punkter.

```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen GlowEffect.Size. Denna egenskap kommer att tas bort 6 månader senare sedan september 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


