---
title: "GradientFill.GradientStops"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GradientFill-Eigenschaft. Stellt die Sammlung von Farbverlaufspunkten dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

Stellt die Sammlung von Gradient-Stops dar.

```csharp
public GradientStopCollection GradientStops { get; }
```

### Beispiele

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
            
            // Rechteckform hinzufügen
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Farbverlauf festlegen
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // Lösche alle vorhandenen Farbverlaufspunkte
            gradientFill.GradientStops.Clear();

            // Füge benutzerdefinierte Farbverlaufspunkte hinzu
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // Demonstriere den Zugriff auf Farbverlaufspunkte
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


