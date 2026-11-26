---
title: "Shape.LeftCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento horizontal de la forma desde su columna izquierda en unidades de centímetros"
type: docs
url: /es/net/aspose.cells.drawing/shape/leftcm/
---
## Shape.LeftCM property

Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de centímetros.

```csharp
public double LeftCM { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftCMDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer y obtener la propiedad LeftCM
            shape.LeftCM = 3.0;
            Console.WriteLine("Shape left position (cm): " + shape.LeftCM);

            // Modificar la posición izquierda si es 3 cm
            if (shape.LeftCM == 3.0)
            {
                shape.LeftCM = 1.0;
                Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


