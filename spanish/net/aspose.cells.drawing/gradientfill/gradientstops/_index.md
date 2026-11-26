---
title: "GradientFill.GradientStops"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientFill. Representa la colección de paradas de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/gradientstops/
---
## GradientFill.GradientStops property

Representa la colección de paradas de degradado.

```csharp
public GradientStopCollection GradientStops { get; }
```

### Ejemplos

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
            
            // Agregar una forma rectangular
            Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Establecer relleno degradado
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            
            // Borrar cualquier parada de degradado existente
            gradientFill.GradientStops.Clear();

            // Agregar paradas de degradado personalizadas
            gradientFill.GradientStops.Add(0.0, Color.Red, 255);
            gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
            gradientFill.GradientStops.Add(1.0, Color.Green, 255);

            // Demostrar el acceso a las paradas de degradado
            Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
            Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
            Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);

            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


