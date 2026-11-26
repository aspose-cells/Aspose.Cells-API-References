---
title: "TextBoxCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TextBoxCollection. Añade un cuadro de texto a la colección"
type: docs
url: /es/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Agrega un cuadro de texto a la colección.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| altura | Int32 | Altura del cuadro de texto, en unidades de píxel. |
| ancho | Int32 | Ancho del cuadro de texto, en unidades de píxel. |

### Valor de retorno

[`TextBox`](../../textbox/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int index = worksheet.TextBoxes.Add(1, 1, 50, 100);
            Console.WriteLine("TextBox added at index: " + index);
        }
    }
}
```

### Ver también

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


