---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore IndividualFontConfigs. Ctor"
type: docs
url: /it/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

Ctor.

```csharp
public IndividualFontConfigs()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento con IndividualFontConfigs
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // Crea una nuova cartella di lavoro con foglio di lavoro predefinito
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // Accedi a un foglio di lavoro e aggiungi del testo
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // Salva la cartella di lavoro (le opzioni di caricamento non sono necessarie per il salvataggio)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### Vedi anche

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


