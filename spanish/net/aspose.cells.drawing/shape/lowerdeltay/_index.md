---
title: "Shape.LowerDeltaY"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene o establece el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha"
type: docs
url: /es/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

Obtiene o establece el desplazamiento vertical de la forma desde la fila de su esquina inferior derecha.

```csharp
public int LowerDeltaY { get; set; }
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
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer y demostrar la propiedad LowerDeltaY
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // Modificar LowerDeltaY condicionalmente
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


