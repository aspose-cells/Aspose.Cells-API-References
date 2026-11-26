---
title: "Shape.UpperLeftRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el índice de la fila superior"
type: docs
url: /es/net/aspose.cells.drawing/shape/upperleftrow/
---
## Shape.UpperLeftRow property

Representa el índice de la fila superior.

```csharp
public int UpperLeftRow { get; set; }
```

### Observaciones

Si la forma está dentro de la forma o en el grupo, UpperLeftRow será ignorado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Establecer y demostrar la propiedad UpperLeftRow
            shape.UpperLeftRow = 3;
            Console.WriteLine("Shape's initial topRow: " + shape.UpperLeftRow);

            // Modificar UpperLeftRow según la condición
            if (shape.UpperLeftRow == 3)
                shape.UpperLeftRow = 1;

            Console.WriteLine("Shape's modified topRow: " + shape.UpperLeftRow);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


