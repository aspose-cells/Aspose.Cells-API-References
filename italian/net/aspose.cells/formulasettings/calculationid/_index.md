---
title: "FormulaSettings.CalculationId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro.

```csharp
public string CalculationId { get; set; }
```

### Osservazioni

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante affinché altre applicazioni (come MS Excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Nel caso di MS Excel, se il valore di questa proprietà è inferiore all'identificatore del motore di ricalcolo associato all'applicazione che apre il file risultante, l'applicazione ricalcolerà i risultati di tutte le formule in questa cartella di lavoro subito dopo il caricamento del file. Per motivi di prestazioni nella maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Imposta una formula che si comporta diversamente in base a CalculationId
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // Calcola senza CalculationId (comportamento predefinito)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // Imposta CalculationId e ricalcola
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


