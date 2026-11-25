---
title: "LoadOptions.AutoFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Indica se filtrare automaticamente i dati durante il caricamento dei file"
type: docs
url: /it/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Indica se filtrare automaticamente i dati durante il caricamento dei file.

```csharp
public bool AutoFilter { get; set; }
```

### Osservazioni

A volte, sebbene l'autofiltro sia impostato, le righe corrispondenti non sono nascoste nel file. Ora funziona solo per i file SpreadSheetML.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento e abilita AutoFilter
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // Carica la cartella di lavoro con AutoFilter abilitato
            Workbook workbook = new Workbook("example.xlsx", options);

            // Accedi al primo foglio di lavoro e applica AutoFilter
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
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


