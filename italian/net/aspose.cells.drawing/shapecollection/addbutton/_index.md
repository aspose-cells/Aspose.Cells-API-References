---
title: "ShapeCollection.AddButton"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge un Button al foglio di lavoro."
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Aggiunge un Button al foglio di lavoro.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale di Button dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale di Button dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza di Button, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza di Button, in unità di pixel. |

### Valore di ritorno

Un oggetto Button.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un pulsante usando i parametri specificati
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Salva la cartella di lavoro
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


