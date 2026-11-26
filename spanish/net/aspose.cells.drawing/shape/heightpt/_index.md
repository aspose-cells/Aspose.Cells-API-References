---
title: "Shape.HeightPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa la altura de la forma en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

Representa la altura de la forma, en unidades de puntos.

```csharp
public double HeightPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // Establecer y obtener la propiedad HeightPt
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // Modificar la altura si coincide con una condición
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


