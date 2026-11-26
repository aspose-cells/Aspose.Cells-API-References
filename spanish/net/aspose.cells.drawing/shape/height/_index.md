---
title: "Shape.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa la altura de la forma en unidades de píxel"
type: docs
url: /es/net/aspose.cells.drawing/shape/height/
---
## Shape.Height property

Representa la altura de la forma, en unidades de píxel.

```csharp
public int Height { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Establecer altura inicial
            shape.Height = 150;
            Console.WriteLine("Initial height: " + shape.Height);

            // Modificar la altura condicionalmente
            if (shape.Height == 150)
            {
                shape.Height = 100;
                Console.WriteLine("Modified height: " + shape.Height);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


