---
title: "Worksheet.ShowFormulas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se mostrare le formule o i loro risultati"
type: docs
url: /it/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Indica se mostrare le formule o i loro risultati.

```csharp
public bool ShowFormulas { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta la formula nella cella A1
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // Mostra inizialmente il valore calcolato
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // Attiva/disattiva la visualizzazione del testo della formula
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


