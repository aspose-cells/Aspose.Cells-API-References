---
title: "GradientStop.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientStop-egenskap. Returnerar eller anger graden av transparens för området som ett värde från 0.0 ogenomskinligt till 1.0 helt genomskinligt"
type: docs
url: /sv/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // Skapa färg för gradientstopp
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // Lägg till gradientstopp med initial transparens
            gradientFill.GradientStops.Add(0, color, 30);

            // Åtkomst till gradientstoppet
            GradientStop stop = gradientFill.GradientStops[0];

            // Visa och ändra transparens
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // Lägg till ett annat stopp för visuell jämförelse
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // Spara arbetsboken
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


