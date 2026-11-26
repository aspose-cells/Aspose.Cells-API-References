---
title: "ShapeCollection.AddListBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Agrega un ListBox a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Agrega un ListBox a la hoja de cálculo.

```csharp
public ListBox AddListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del ListBox desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del ListBox desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del ListBox, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del ListBox, en unidades de píxel. |

### Valor de retorno

Un objeto ListBox.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddListBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de lista a la hoja de cálculo
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 50);

            // Agregar elementos al cuadro de lista
            listBox.SetInputRange("A1:A3", false, false);
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Guarda el libro de trabajo
            workbook.Save("ListBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListBox](../../listbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


