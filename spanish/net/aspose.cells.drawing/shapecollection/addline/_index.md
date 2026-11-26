---
title: "ShapeCollection.AddLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un LineShape a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addline/
---
## ShapeCollection.AddLine method

Agrega una LineShape a la hoja de cálculo.

```csharp
public LineShape AddLine(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del LineShape desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del LineShape desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del LineShape, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del LineShape, en unidades de píxel. |

### Valor de retorno

Un objeto LineShape.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLineWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [LineShape](../../lineshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


