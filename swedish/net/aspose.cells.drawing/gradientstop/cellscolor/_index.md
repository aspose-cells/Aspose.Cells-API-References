---
title: "GradientStop.CellsColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientStop-egenskap. Hämtar färgen på detta gradientstopp"
type: docs
url: /sv/net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

Hämtar färgen på detta gradientstopp.

```csharp
public CellsColor CellsColor { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
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

                // Åtkomst till gradientstoppet och visa dess CellsColor-egenskaper
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // Spara arbetsboken
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


