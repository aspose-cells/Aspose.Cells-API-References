---
title: "ShapeCollection.AddSpinner"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Aggiunge uno Spinner al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Aggiunge un Spinner al foglio di lavoro.

```csharp
public Spinner AddSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale dello Spinner dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale dello Spinner dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza dello Spinner, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza dello Spinner, in unità di pixel. |

### Valore di ritorno

Un oggetto Spinner.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSpinnerWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno spinner al foglio di lavoro
            Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);

            // Imposta le proprietà del spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 1;

            // Salva la cartella di lavoro
            workbook.Save("AddSpinnerDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


