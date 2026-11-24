---
title: "ShadowEffect.Distance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShadowEffect-Eigenschaft. Gibt den Abstand des Schattens zurück und legt ihn fest. Bereich von 0 bis 200 Punkten"
type: docs
url: /de/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Liest und setzt den Abstand des Schattens. Bereich von 0 bis 200 Punkten.

```csharp
public double Distance { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck hinzu
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // Konfiguriere den Schatteneffekt
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // Erstelle ein CellsColor-Objekt und setze ARGB-Werte
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // Zeige den Schattenabstand an
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // Speichere das Arbeitsbuch mit Schatteneffekt
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


