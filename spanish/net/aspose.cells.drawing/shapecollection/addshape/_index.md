---
title: "ShapeCollection.AddShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega una Forma a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addshape/
---
## ShapeCollection.AddShape method

Agrega una Shape a la hoja de cálculo.

```csharp
public Shape AddShape(MsoDrawingType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | MsoDrawingType | Tipo de dibujo Mso. |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura de Shape, en unidades de píxel. |
| ancho | Int32 | Representa el ancho de Shape, en unidades de píxel. |

### Valor de retorno

Un objeto Shape.

### Observaciones

El tipo no pudo ser Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 200, 50);
            
            Console.WriteLine("Shape added successfully.");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


