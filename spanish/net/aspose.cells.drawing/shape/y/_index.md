---
title: "Shape.Y"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene y establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

Obtiene y establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

```csharp
public int Y { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Establecer y demostrar la propiedad Y
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // Modificar la posición Y según la condición
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


