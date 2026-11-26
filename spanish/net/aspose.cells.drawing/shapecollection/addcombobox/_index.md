---
title: "ShapeCollection.AddComboBox"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade un ComboBox a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Agrega un ComboBox a la hoja de cálculo.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical del ComboBox desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal del ComboBox desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura del ComboBox, en unidades de píxel. |
| ancho | Int32 | Representa el ancho del ComboBox, en unidades de píxel. |

### Valor de retorno

Un objeto ComboBox.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar un combo box con los parámetros especificados
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Agregar elementos al combo box estableciendo valores de celda
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Establecer el rango de entrada para el cuadro combinado
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Guarda el libro de trabajo
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


