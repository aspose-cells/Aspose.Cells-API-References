---
title: "Enum GradientFillType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GradientFillType enum. Representerar alla gradientfyllningstyper"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Representerar alla fyllningstyper för gradient.

```csharp
public enum GradientFillType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Linear | `0` | Linjär |
| Radial | `1` | Radial |
| Rectangle | `2` | Rektangel |
| Path | `3` | Sökväg |

### Exempel

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

            // Skapa en form för att demonstrera gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // Hämta fyllningsformatet
            FillFormat fillFormat = shape.Fill;

            // Ställ in gradientfyllningstyp och egenskaper
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Skriv ut gradientriktningstyp
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Spara arbetsboken
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


