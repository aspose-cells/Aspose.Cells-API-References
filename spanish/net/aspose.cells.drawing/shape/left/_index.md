---
title: "Shape.Left"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento horizontal de la forma desde su columna izquierda en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxeles.

```csharp
public int Left { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar la propiedad Left
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Establecer la posición inicial Left
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // Modificar la posición Left condicionalmente
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


