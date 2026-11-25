---
title: "TextBoxCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TextBoxCollection. Rimuove una casella di testo dal file"
type: docs
url: /it/net/aspose.cells.drawing/textboxcollection/removeat/
---
## TextBoxCollection.RemoveAt method

Rimuovi una casella di testo dal file.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice della casella di testo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcune caselle di testo al foglio di lavoro
            for (int i = 0; i < 3; i++)
            {
                worksheet.TextBoxes.Add(10, 10 + (i * 30), 200, 50);
                worksheet.TextBoxes[i].Text = "TextBox " + (i + 1);
            }

            Console.WriteLine("Before removal - TextBox count: " + worksheet.TextBoxes.Count);

            // Rimuovi l'ultima casella di testo usando RemoveAt con parametro Int32
            int lastIndex = worksheet.TextBoxes.Count - 1;
            worksheet.TextBoxes.RemoveAt(lastIndex);

            Console.WriteLine("After removal - TextBox count: " + worksheet.TextBoxes.Count);
        }
    }
}
```

### Vedi anche

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


