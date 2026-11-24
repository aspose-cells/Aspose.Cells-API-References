---
title: "Enum GradientFillType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GradientFillType enum. Stellt alle Gradient-Fülltypen dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Stellt alle Gradient-Fülltypen dar.

```csharp
public enum GradientFillType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Linear | `0` | Linear |
| Radial | `1` | Radial |
| Rectangle | `2` | Rechteck |
| Path | `3` | Pfad |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Form, um die Gradientfüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // Hole das Füllformat
            FillFormat fillFormat = shape.Fill;

            // Setze den Gradientfülltyp und die Eigenschaften
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Gib den Gradient-Richtungstyp aus
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Speichere die Arbeitsmappe
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


