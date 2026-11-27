---
title: "Klass GradientStop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GradientStop-klass. Representerar gradientstoppet"
type: docs
url: /sv/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Representerar gradientstopp.

```csharp
public class GradientStop
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Hämtar färgen på detta gradientstopp. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | Positionen för stoppet. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en form med gradientfyllning
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Skapa färg för gradientstopp
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Lägg till gradientstopp
                gradientFill.GradientStops.Add(0, color, 30);

                // Åtkomst till gradientstoppet
                GradientStop stop = gradientFill.GradientStops[0];

                // Demonstrera grundläggande funktionalitet
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Ändra egenskaper
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Spara arbetsboken
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


