---
title: "ShapeCollection.AddOval"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un Oval a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addoval/
---
## ShapeCollection.AddOval method

Agrega una Oval a la hoja de cálculo.

```csharp
public Oval AddOval(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del Oval desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del Oval desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del Oval, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del Oval, en unidades de píxel. |

### Valor de retorno

Un objeto Oval.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOvalWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma ovalada a la hoja de cálculo
            ShapeCollection shapes = worksheet.Shapes;
            Oval oval = shapes.AddOval(1, 0, 1, 0, 50, 50);

            // Guarda el libro de trabajo
            workbook.Save("AddOvalDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Oval](../../oval/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


