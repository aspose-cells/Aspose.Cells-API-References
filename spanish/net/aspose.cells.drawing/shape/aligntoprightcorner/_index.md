---
title: "Shape.AlignTopRightCorner"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Shape. Mueve la imagen a la esquina superior derecha"
type: docs
url: /es/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

Mueve la imagen a la esquina superior derecha.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | el índice de fila. |
| rightColumn | Int32 | el índice de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape de muestra para alinear
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Alinear la esquina superior derecha del shape a la fila 2, columna 5
            shape.AlignTopRightCorner(2, 5);

            // Guarda el libro de trabajo
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


