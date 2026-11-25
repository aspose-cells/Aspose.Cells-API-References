---
title: "LoadOptions.FontConfigs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene e imposta le configurazioni dei caratteri individuali. Funziona solo per il Workbook che utilizza queste LoadOptions per il caricamento"
type: docs
url: /it/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

Ottiene e imposta le configurazioni dei caratteri individuali. Funziona solo per il [`Workbook`](../../workbook/) che utilizza questo [`LoadOptions`](../) per il caricamento.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyFontConfigsDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento con FontConfigs
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // Imposta alcune regole di sostituzione dei caratteri utilizzando l'API corretta
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // Carica un file CSV con le opzioni specificate
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


