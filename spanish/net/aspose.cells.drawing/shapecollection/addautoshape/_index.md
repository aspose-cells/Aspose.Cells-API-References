---
title: "ShapeCollection.AddAutoShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un AutoShape a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Agrega una AutoShape a la hoja de cálculo.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | AutoShapeType | Tipo de AutoShape. |
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
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


