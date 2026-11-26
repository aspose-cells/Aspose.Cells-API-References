---
title: "ShapeCollection.AddTextBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapeCollection método. Agrega un cuadro de texto a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Agrega un cuadro de texto a la hoja de cálculo.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del cuadro de texto desde su fila superior, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del cuadro de texto desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del cuadro de texto, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del cuadro de texto, en unidades de píxel. |

### Valor de retorno

Un objeto [`TextBox`](../../textbox/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar un TextBox con posición y tamaño especificados
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Guarda el libro de trabajo
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


