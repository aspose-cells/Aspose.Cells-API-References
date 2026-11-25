---
title: "FormulaSettings.CalculateOnSave"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Indica se ricalcolare la cartella di lavoro prima di salvare il documento quando è in modalità di calcolo manuale"
type: docs
url: /it/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Indica se ricalcolare la cartella di lavoro prima di salvare il documento, quando è in modalità di calcolo manuale.

```csharp
public bool CalculateOnSave { get; set; }
```

### Osservazioni

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante affinché altre applicazioni (come MS Excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni nella maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al foglio di lavoro e aggiungi alcuni dati
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Disabilita CalculateOnSave (il valore predefinito è false)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Salva senza calcolare le formule
            workbook.Save("output_without_calculation.xlsx");

            // Abilita CalculateOnSave
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Salva con il calcolo delle formule
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


