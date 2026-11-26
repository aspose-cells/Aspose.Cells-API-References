---
title: "Shape.MoveToRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Mueve la forma a un rango especificado"
type: docs
url: /es/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Mueve la forma a un rango especificado.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| bottomRow | Int32 | Índice de fila inferior derecha |
| rightColumn | Int32 | Índice de columna inferior derecha |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Mueva la forma a un rango específico
            shape.MoveToRange(12, 3, 13, 5);

            // Guarda el libro de trabajo
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


