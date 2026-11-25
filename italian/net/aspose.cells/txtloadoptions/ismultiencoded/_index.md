---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. True indica che il file contiene diverse codifiche"
type: docs
url: /it/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

True indica che il file contiene diverse codifiche.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento del testo
            TxtLoadOptions options = new TxtLoadOptions();
            
            // Imposta IsMultiEncoded su true per gestire più codifiche
            options.IsMultiEncoded = true;
            
            // Carica la cartella di lavoro con le opzioni
            Workbook workbook = new Workbook("example.csv", options);
            
            // Visualizza i valori di esempio dal file caricato
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


