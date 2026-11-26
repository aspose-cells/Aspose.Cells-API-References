---
title: "Shape.LowerDeltaX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene o establece el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha"
type: docs
url: /es/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

Obtiene o establece el desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha.

```csharp
public int LowerDeltaX { get; set; }
```

### Observaciones

El rango de valores es de 0 a 1024.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer y demostrar la propiedad LowerDeltaX
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // Modificar LowerDeltaX si se cumple la condición
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


