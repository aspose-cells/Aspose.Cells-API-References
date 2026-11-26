---
title: "Shape.UpperDeltaY"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene o establece el desplazamiento vertical de la forma desde su fila de esquina superior izquierda"
type: docs
url: /es/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

Obtiene o establece el desplazamiento vertical de la forma desde la fila de su esquina superior izquierda.

```csharp
public int UpperDeltaY { get; set; }
```

### Observaciones

El rango de valor es de 0 a 256.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar la propiedad UpperDeltaY
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer y mostrar el valor inicial de UpperDeltaY
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // Modificar el valor de UpperDeltaY
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


