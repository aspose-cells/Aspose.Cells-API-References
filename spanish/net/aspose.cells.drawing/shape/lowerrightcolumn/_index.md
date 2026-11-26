---
title: "Shape.LowerRightColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Representa el índice de columna de la esquina inferior derecha"
type: docs
url: /es/net/aspose.cells.drawing/shape/lowerrightcolumn/
---
## Shape.LowerRightColumn property

Representa el índice de columna de la esquina inferior derecha.

```csharp
public int LowerRightColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Establecer y mostrar el valor inicial de LowerRightColumn
            shape.LowerRightColumn = 3;
            Console.WriteLine("Initial LowerRightColumn: " + shape.LowerRightColumn);

            // Modificar LowerRightColumn si es igual a 3
            if (shape.LowerRightColumn == 3)
            {
                shape.LowerRightColumn = 1;
                Console.WriteLine("Modified LowerRightColumn: " + shape.LowerRightColumn);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


