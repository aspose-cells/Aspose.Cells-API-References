---
title: "Shape.UpperDeltaX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene o establece el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda"
type: docs
url: /es/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

Obtiene o establece el desplazamiento horizontal de la forma desde la columna de su esquina superior izquierda.

```csharp
public int UpperDeltaX { get; set; }
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
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Establecer y mostrar la propiedad UpperDeltaX
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // Modificar la UpperDeltaX si cumple una condición
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


