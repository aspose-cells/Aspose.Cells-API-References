---
title: "Spinner.CurrentValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Spinner. Ottiene o imposta il valore corrente"
type: docs
url: /it/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Ottiene o imposta il valore corrente.

```csharp
public int CurrentValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo spinner
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // Imposta le proprietà del spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // Verifica e visualizza il valore corrente
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // Salva la cartella di lavoro
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


