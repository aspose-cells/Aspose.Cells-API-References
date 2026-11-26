---
title: "Shape.UpperLeftColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el índice de columna de la esquina superior izquierda"
type: docs
url: /es/net/aspose.cells.drawing/shape/upperleftcolumn/
---
## Shape.UpperLeftColumn property

Representa el índice de columna de la esquina superior izquierda.

```csharp
public int UpperLeftColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma a la hoja de cálculo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100);

            // Establecer y demostrar la propiedad UpperLeftColumn
            shape.UpperLeftColumn = 3;
            Console.WriteLine("Shape's initial leftColumn: " + shape.UpperLeftColumn);

            // Modificar el UpperLeftColumn
            if (shape.UpperLeftColumn == 3)
            {
                shape.UpperLeftColumn = 1;
                Console.WriteLine("Shape's modified leftColumn: " + shape.UpperLeftColumn);
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeUpperLeftColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


