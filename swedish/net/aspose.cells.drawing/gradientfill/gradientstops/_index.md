---
title: "GradientFill.GradientStops"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill property. Representerar samlingen av gradientstopp"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

Representerar samlingen av gradientstopp.

```csharp
public GradientStopCollection GradientStops { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyGradientStopsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;
            
            // Lägg till en rektangelform
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Ställ in gradientfyllning
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // Rensa eventuella befintliga gradientstopp
            gradientFill.GradientStops.Clear();

            // Lägg till anpassade gradientstopp
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // Demonstrera åtkomst till gradientstopp
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


