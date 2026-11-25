---
title: "TextBoxCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TextBoxCollection. Aggiunge una casella di testo alla collezione"
type: docs
url: /it/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Aggiunge un textbox alla collezione.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| altezza | Int32 | Altezza della casella di testo, in unità di pixel. |
| larghezza | Int32 | Larghezza della casella di testo, in unità di pixel. |

### Valore di ritorno

[`TextBox`](../../textbox/) object index.

### Esempi

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

### Vedi anche

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


