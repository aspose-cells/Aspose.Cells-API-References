---
title: "ShapeCollection.AddLabel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade una etiqueta a la hoja de cálculo."
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Agrega una Etiqueta a la hoja de cálculo.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de la etiqueta desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal de la etiqueta desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura de la etiqueta, en unidades de píxel. |
| ancho | Int32 | Representa el ancho de la etiqueta, en unidades de píxel. |

### Valor de retorno

Un objeto Label.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Añade una etiqueta a la hoja de cálculo
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // Guarda el libro de trabajo
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


