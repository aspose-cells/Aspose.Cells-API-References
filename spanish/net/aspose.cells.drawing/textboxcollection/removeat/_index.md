---
title: "TextBoxCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TextBoxCollection. Elimina un cuadro de texto del archivo"
type: docs
url: /es/net/aspose.cells.drawing/textboxcollection/removeat/
---
## TextBoxCollection.RemoveAt method

Eliminar un cuadro de texto del archivo.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del cuadro de texto. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añada algunos cuadros de texto a la hoja de cálculo
            for (int i = 0; i < 3; i++)
            {
                worksheet.TextBoxes.Add(10, 10 + (i * 30), 200, 50);
                worksheet.TextBoxes[i].Text = "TextBox " + (i + 1);
            }

            Console.WriteLine("Before removal - TextBox count: " + worksheet.TextBoxes.Count);

            // Elimine el último cuadro de texto usando RemoveAt con el parámetro Int32
            int lastIndex = worksheet.TextBoxes.Count - 1;
            worksheet.TextBoxes.RemoveAt(lastIndex);

            Console.WriteLine("After removal - TextBox count: " + worksheet.TextBoxes.Count);
        }
    }
}
```

### Ver también

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


