---
title: "ShapeCollection.AddRadioButton"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapeCollection metodo. Aggiunge un RadioButton al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addradiobutton/
---
## ShapeCollection.AddRadioButton method

Aggiunge un RadioButton al foglio di lavoro.

```csharp
public RadioButton AddRadioButton(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale del RadioButton dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale del RadioButton dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza del RadioButton, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza del RadioButton, in unità di pixel. |

### Valore di ritorno

Un oggetto RadioButton.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRadioButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un pulsante di opzione al foglio di lavoro
            Aspose.Cells.Drawing.RadioButton radioButton = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
            radioButton.Text = "Option 1";

            // Salva la cartella di lavoro
            workbook.Save("RadioButtonDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RadioButton](../../radiobutton/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


