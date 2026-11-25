---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Indica se analizzare la formula durante la lettura del file"
type: docs
url: /it/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Indica se analizzare la formula durante la lettura del file.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Osservazioni

Si applica solo ai file Excel Xlsx, Xltx, Xltm e Xlsm perché le formule nei file sono memorizzate come stringa di formula.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento
            LoadOptions loadOptions = new LoadOptions();
            
            // Imposta ParsingFormulaOnOpen su false per saltare l'analisi delle formule durante il caricamento
            loadOptions.ParsingFormulaOnOpen = false;
            
            // Carica la cartella di lavoro con le opzioni specificate
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // Accedi al foglio di lavoro e dimostra che l'analisi delle formule è stata saltata
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


