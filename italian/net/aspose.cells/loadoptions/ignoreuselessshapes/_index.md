---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Indica se ignorare le forme inutili"
type: docs
url: /it/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Indica se ignorare forme inutili.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Osservazioni

Funziona solo per i file xlsx, xlsb e xlsm. Ci sono molte forme identiche sovrapposte che sono inutili in alcuni file; possiamo ignorarle durante il caricamento dei file.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento e imposta IgnoreUselessShapes su true
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // Carica la cartella di lavoro con le opzioni
            Workbook workbook = new Workbook("example.xlsx", options);

            // Restituisci il conteggio delle forme nel primo foglio di lavoro
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


