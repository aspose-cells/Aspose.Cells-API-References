---
title: "LoadOptions.WarningCallback"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta il callback di avviso"
type: docs
url: /it/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Ottiene o imposta il callback di avviso.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crea un callback di avviso personalizzato
            IWarningCallback warningCallback = new CustomWarningCallback();

            // Inizializza le opzioni di caricamento con il callback di avviso
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // Carica la cartella di lavoro con opzioni
            Workbook workbook = new Workbook("example.xlsx", options);

            // Dimostra l'uso del callback di avviso accedendo a una cella
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


