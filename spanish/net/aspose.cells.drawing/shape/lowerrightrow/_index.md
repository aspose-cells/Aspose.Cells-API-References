---
title: "Shape.LowerRightRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el índice de fila de la esquina inferior derecha"
type: docs
url: /es/net/aspose.cells.drawing/shape/lowerrightrow/
---
## Shape.LowerRightRow property

Representa el índice de fila de la esquina inferior derecha.

```csharp
public int LowerRightRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer y demostrar la propiedad LowerRightRow
            Console.WriteLine("Original LowerRightRow: " + shape.LowerRightRow);
            shape.LowerRightRow = 3;
            Console.WriteLine("Modified LowerRightRow: " + shape.LowerRightRow);

            // Modificación condicional según el caso de prueba
            if (shape.LowerRightRow == 3)
            {
                shape.LowerRightRow = 1;
                Console.WriteLine("Final LowerRightRow after condition: " + shape.LowerRightRow);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


