---
title: "Shape.X"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene y establece el desplazamiento horizontal del shape desde el borde izquierdo de la hoja de cálculo en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

Obtiene y establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo, en unidades de píxeles.

```csharp
public int X { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Establecer la posición X inicial
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // Modificar la posición X si es igual a 3 (demostrando la lógica del caso de prueba)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // Para demostración, cambiar la posición X a 300
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


