---
title: "GradientFill.DirectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill-egenskap. Hämtar gradientens riktnings typ"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Hämtar gradientens riktningstyp.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att demonstrera gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // Ställ in gradientfyllningsegenskaper
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Skriv ut gradientens riktningstyp
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Spara arbetsboken
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### Se även

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


