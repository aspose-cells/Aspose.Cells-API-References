---
title: "Shape.Placement"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shape/placement/
---
## Shape.Placement property

Representa la forma en que el objeto de dibujo está unido a las celdas debajo de él. La propiedad controla la ubicación de un objeto en una hoja de cálculo.

```csharp
public PlacementType Placement { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyPlacementDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);

            // Demostrar la propiedad Placement
            Console.WriteLine("Original Placement: " + shape.Placement);
            
            // Cambiar el tipo de ubicación
            shape.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Modified Placement: " + shape.Placement);

            // Guarda el libro de trabajo
            workbook.Save("ShapePlacementDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


