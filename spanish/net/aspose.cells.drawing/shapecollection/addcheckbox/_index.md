---
title: "ShapeCollection.AddCheckBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade una casilla de verificación a la hoja de cálculo."
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addcheckbox/
---
## ShapeCollection.AddCheckBox method

Agrega una casilla de verificación a la hoja de cálculo.

```csharp
public CheckBox AddCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de la casilla de verificación desde su fila superior, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del cuadro de texto desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Altura del cuadro de texto, en unidades de píxel. |
| ancho | Int32 | Ancho del cuadro de texto, en unidades de píxel. |

### Valor de retorno

El índice del nuevo objeto CheckBox.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCheckBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Añade una CheckBox usando los parámetros especificados
            Aspose.Cells.Drawing.CheckBox checkBox = shapes.AddCheckBox(1, 0, 1, 0, 100, 50);

            // Guarda el libro de trabajo
            workbook.Save("CheckBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBox](../../checkbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


