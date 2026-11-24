---
title: "ShadowEffect.Size"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShadowEffect-Eigenschaft. Gibt die Größe des Schattens zurück und legt sie fest. Bereich von 0 bis 2,0. Bedeutungslose im inneren Schatten"
type: docs
url: /de/net/aspose.cells.drawing/shadoweffect/size/
---
## ShadowEffect.Size property

Liest und setzt die Größe des Schattens. Bereich von 0 bis 2,0. Bedeutungslose bei innerem Schatten.

```csharp
public double Size { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertySizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook book = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge eine Form hinzu
            Worksheet sheet = book.Worksheets[0];
            Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Hole den Schatteneffekt und setze Eigenschaften, einschließlich Größe
            ShadowEffect shadow = shape.ShadowEffect;
            shadow.Angle = 150;
            shadow.Blur = 30;
            shadow.Size = 1.3; // Demonstrating Size property usage
            shadow.Transparency = 0.4;
            shadow.Distance = 80;

            // Speichere die Arbeitsmappe
            book.Save("ShadowEffectExample.xlsx");
            
            Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
        }
    }
}
```

### Siehe auch

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


