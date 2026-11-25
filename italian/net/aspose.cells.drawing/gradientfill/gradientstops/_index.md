---
title: "GradientFill.GradientStops"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GradientFill. Rappresenta la raccolta di fermate del gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

Rappresenta la raccolta di punti di arresto del gradiente.

```csharp
public GradientStopCollection GradientStops { get; }
```

### Esempi

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
            
            // Aggiungi una forma rettangolare
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Imposta il riempimento gradiente
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // Cancella eventuali fermate del gradiente esistenti
            gradientFill.GradientStops.Clear();

            // Aggiungi fermate del gradiente personalizzate
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // Dimostra l'accesso alle fermate del gradiente
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


