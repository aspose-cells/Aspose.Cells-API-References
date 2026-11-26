---
title: "ShapeCollection.AddRectangle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade un RectangleShape a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addrectangle/
---
## ShapeCollection.AddRectangle method

Agrega una RectangleShape a la hoja de cálculo.

```csharp
public RectangleShape AddRectangle(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del RectangleShape desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal de RectangleShape desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura de RectangleShape, en unidades de píxel. |
| ancho | Int32 | Representa el ancho de RectangleShape, en unidades de píxel. |

### Valor de retorno

Un objeto RectangleShape.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRectangleWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade un rectángulo usando los parámetros especificados
            RectangleShape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Guarda el libro de trabajo
            workbook.Save("RectangleShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RectangleShape](../../rectangleshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


