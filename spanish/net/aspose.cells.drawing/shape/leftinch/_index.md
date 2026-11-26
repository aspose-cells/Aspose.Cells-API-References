---
title: "Shape.LeftInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento horizontal de la forma desde su columna izquierda en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de pulgadas.

```csharp
public double LeftInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Establecer y demostrar la propiedad LeftInch
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // Modificar la posición izquierda si es 3 pulgadas
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


