---
title: "GradientFill.Angle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill egenskap. Vinkeln för linjär fyllning"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/angle/
---
## GradientFill.Angle property

Vinkeln för linjär fyllning.

```csharp
public float Angle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Ställ in gradientfyllningsegenskaper
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromCenter);
            shape.Fill.GradientFill.Angle = 45; // Set the angle to 45 degrees

            // Ställ in gradientfärger
            shape.Fill.GradientFill.SetTwoColorGradient(
                Color.Red, 
                Color.Blue, 
                GradientStyleType.Horizontal, 
                1);

            // Spara arbetsboken
            workbook.Save("GradientFillAngleDemo.xlsx");

            Console.WriteLine("Demo completed. File saved with gradient fill at 45 degree angle.");
        }
    }
}
```

### Se även

* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


