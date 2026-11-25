---
title: "LoadOptions.KeepUnparsedData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Indica se mantenere i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Indica se mantenere i dati non analizzati in memoria per il Workbook quando viene caricato da un file modello. Il valore predefinito è true.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Osservazioni

Per scenari in cui l'utente deve solo leggere alcuni contenuti dal file modello e non ha bisogno di salvare nuovamente la cartella di lavoro, impostare questa proprietà su false può migliorare le prestazioni, soprattutto quando la si utilizza insieme a qualche tipo di LoadFilter,

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento e imposta KeepUnparsedData su false
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // Carica la cartella di lavoro con opzioni
            Workbook workbook = new Workbook("example.xlsx", options);

            // Accedi al foglio di lavoro e dimostra che i dati non analizzati non vengono conservati
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


