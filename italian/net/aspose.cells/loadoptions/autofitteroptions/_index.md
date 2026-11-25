---
title: "LoadOptions.AutoFitterOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene e imposta le opzioni di auto‑adattamento"
type: docs
url: /it/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Ottiene e imposta le opzioni dell'auto fitter

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Osservazioni

Solo per file xlsx, spreadsheetML al momento.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Crea AutoFitterOptions e imposta le proprietà
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // Crea LoadOptions e assegna AutoFitterOptions
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // Carica la cartella di lavoro con le opzioni specificate
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // Dimostra l'auto‑adattamento ottenendo l'altezza della riga
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


