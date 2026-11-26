---
title: "ShapeCollection.AddArc"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un ArcShape a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Agrega una ArcShape a la hoja de cálculo.

```csharp
public ArcShape AddArc(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del ArcShape desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del ArcShape desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del ArcShape, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del ArcShape, en unidades de píxel. |

### Valor de retorno

Un objeto ArcShape.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
            
            workbook.Save("AddArcDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


