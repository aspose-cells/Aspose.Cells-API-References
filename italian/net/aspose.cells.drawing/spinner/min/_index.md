---
title: "Spinner.Min"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Spinner. Ottiene o imposta il valore minimo di una barra di scorrimento o dell'intervallo dello spinner"
type: docs
url: /it/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

Ottiene o imposta il valore minimo dell'intervallo di una barra di scorrimento o di uno spinner.

```csharp
public int Min { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMinDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo spinner con le dimensioni corrette
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // Imposta le proprietà dello spinner includendo Min
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // Verifica e visualizza la proprietà Min
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // Salva la cartella di lavoro
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


