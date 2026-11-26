---
title: "Shape.Width"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el ancho de la forma en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/width/
---
## Shape.Width property

Representa el ancho de la forma, en unidades de píxeles.

```csharp
public int Width { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);

            // Establecer el ancho inicial y mostrarlo
            shape.Width = 300;
            Console.WriteLine("Initial width: " + shape.Width);

            // Modificar el ancho según la condición
            if (shape.Width == 300)
                shape.Width = 150;

            Console.WriteLine("Modified width: " + shape.Width);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


