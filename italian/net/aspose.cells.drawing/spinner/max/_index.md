---
title: "Spinner.Max"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Spinner. Ottiene o imposta il valore massimo di una barra di scorrimento o dell'intervallo dello spinner"
type: docs
url: /it/net/aspose.cells.drawing/spinner/max/
---
## Spinner.Max property

Ottiene o imposta il valore massimo dell'intervallo di una barra di scorrimento o di uno spinner.

```csharp
public int Max { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMaxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Spinner spinner = sheet.Shapes.AddSpinner(1, 1, 0, 0, 100, 100);
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;

            Console.WriteLine($"Spinner Max Value: {spinner.Max}");
        }
    }
}
```

### Vedi anche

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


