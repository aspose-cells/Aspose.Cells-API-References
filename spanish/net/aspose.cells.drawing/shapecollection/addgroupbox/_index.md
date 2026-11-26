---
title: "ShapeCollection.AddGroupBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapeCollection método. Añade un GroupBox a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Agrega un GroupBox a la hoja de cálculo.

```csharp
public GroupBox AddGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del GroupBox desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del GroupBox desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del GroupBox, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del GroupBox, en unidades de píxel. |

### Valor de retorno

Un objeto GroupBox.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddGroupBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un group box a la hoja de cálculo
            ShapeCollection shapes = worksheet.Shapes;
            Aspose.Cells.Drawing.GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);

            // Guarda el libro de trabajo
            workbook.Save("GroupBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


