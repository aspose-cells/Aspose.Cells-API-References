---
title: "Klasse GlowEffect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GlowEffect Klasse. Diese Klasse definiert einen Leuchteffekt, bei dem ein farblich verschwommener Umriss außerhalb der Objektkanten hinzugefügt wird."
type: docs
url: /de/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

Diese Klasse definiert einen Leuchteffekt, bei dem ein farblich verschwommener Umriss außerhalb der Kanten des Objekts hinzugefügt wird.

```csharp
public class GlowEffect
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Liest die Farbe des Leuchteffekts. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolete.**) Liest und setzt den Radius des Leuchteffekts in Punkten. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Liest und setzt den Radius des Leuchteffekts in Punkten. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Liest und setzt den Transparenzgrad des Leuchteffekts. Bereich von 0,0 (undurchsichtig) bis 1,0 (transparent). |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie dem Arbeitsblatt eine Bogenform hinzu
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Setzen Sie die Platzierung des Bogens
            arcShape.Placement = PlacementType.FreeFloating;

            // Setzen Sie das Füllformat
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Setzen Sie den Linienstil
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Erstellen Sie eine GlowEffect-Instanz und setzen Sie deren Eigenschaften
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Speichere die Arbeitsmappe
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


