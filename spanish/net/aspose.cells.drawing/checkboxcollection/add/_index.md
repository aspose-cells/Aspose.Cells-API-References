---
title: "CheckBoxCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CheckBoxCollection. Añade un checkBox a la colección"
type: docs
url: /es/net/aspose.cells.drawing/checkboxcollection/add/
---
## CheckBoxCollection.Add method

Agrega un checkBox a la colección.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| altura | Int32 | Altura del checkBox, en unidades de píxel. |
| ancho | Int32 | Ancho del checkBox, en unidades de píxel. |

### Valor de retorno

[`CheckBox`](../../checkbox/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar checkbox usando parámetros Int32 (upperLeftRow, upperLeftColumn, height, width)
            int index = worksheet.CheckBoxes.Add(10, 2, 20, 100);
            
            CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Value = true;
            checkBox.LinkedCell = "B11";
            
            workbook.Save("CheckBoxDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


