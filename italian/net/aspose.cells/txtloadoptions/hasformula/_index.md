---
title: "TxtLoadOptions.HasFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Indica se il testo è una formula se inizia con"
type: docs
url: /it/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

Indica se il testo è una formula se inizia con "=\".

```csharp
public bool HasFormula { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento del testo e abilita l'analisi delle formule
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // Carica la cartella di lavoro con formule nel file di testo
            Workbook workbook = new Workbook("example.csv", options);
            
            // Accedi a una cella con formula e visualizzala
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // Salva la cartella di lavoro
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


