---
title: "ShapeCollection.AddTextBox"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge una casella di testo al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Aggiunge una casella di testo al foglio di lavoro.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale della casella di testo dalla sua riga superiore, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale della casella di testo dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza della casella di testo, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza della casella di testo, in unità di pixel. |

### Valore di ritorno

Un oggetto [`TextBox`](../../textbox/).

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi una TextBox con posizione e dimensioni specificate
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Salva la cartella di lavoro
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


