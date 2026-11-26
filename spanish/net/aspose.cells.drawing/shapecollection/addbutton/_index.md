---
title: "ShapeCollection.AddButton"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un Button a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Agrega un botón a la hoja de cálculo.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del Button desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del Button desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del Button, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del Button, en unidades de píxel. |

### Valor de retorno

Un objeto Button.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un botón usando los parámetros especificados
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Guarda el libro de trabajo
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


