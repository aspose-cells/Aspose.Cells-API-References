---
title: "GradientFill.DirectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GradientFill-Eigenschaft. Gibt den Verlaufrichtungstyp zurück."
type: docs
url: /de/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Liest den Verlauf-Richtungstyp.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Form, um die Gradientfüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // Setze Verlauffüllungseigenschaften.
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Geben Sie den Farbverlaufsrichtungstyp aus
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Speichere die Arbeitsmappe
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


