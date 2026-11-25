---
title: "Spinner.IncrementalChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Spinner. Ottiene o imposta la quantità di incremento della barra di scorrimento o dello spinner per una linea di scorrimento"
type: docs
url: /it/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Ottiene o imposta la quantità di incremento della barra di scorrimento o dello spinner per una linea di scorrimento.

```csharp
public int IncrementalChange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un controllo spinner
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // Imposta le proprietà del spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // Verifica e visualizza il valore IncrementalChange
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // Modifica e verifica nuovamente
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // Salva la cartella di lavoro
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


