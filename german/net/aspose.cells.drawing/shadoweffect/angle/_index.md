---
title: "ShadowEffect.Angle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShadowEffect-Eigenschaft. Gibt den Beleuchtungswinkel zurück und legt ihn fest. Bereich von 0 bis 359,9 Grad"
type: docs
url: /de/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Liest und setzt den Beleuchtungswinkel. Bereich von 0 bis 359,9 Grad.

```csharp
public double Angle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu und setze den Schatteneffektwinkel
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // Überprüfe und gib den Winkelwert aus
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


