---
title: "Klass GlowEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GlowEffect-klass. Denna klass specificerar en glödeffekt där en färgad suddig kontur läggs till utanför objektets kanter."
type: docs
url: /sv/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

Denna klass specificerar en glödeffekt, där en färgad suddig kontur läggs till utanför objektets kanter.

```csharp
public class GlowEffect
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Hämtar färgen på glödeffekten. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolete.**) Hämtar och anger glödens radie i enheter av punkter. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Hämtar och anger glödens radie i enheter av punkter. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Hämtar och anger graden av transparens för glödeffekten. Omfång från 0,0 (opak) till 1,0 (klar). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GlowEffectDemo
    {
        public static void GlowEffectExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bågform till kalkylbladet
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Ange placeringen av bågen
            arcShape.Placement = PlacementType.FreeFloating;

            // Ange fyllningsformatet
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Ange linjestilen
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Skapa en GlowEffect-instans och ange dess egenskaper
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Spara arbetsboken
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


