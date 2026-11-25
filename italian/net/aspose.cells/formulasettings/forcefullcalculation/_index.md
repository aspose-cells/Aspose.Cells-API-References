---
title: "FormulaSettings.ForceFullCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Indica se calcola tutte le formule ogni volta quando viene avviato un calcolo"
type: docs
url: /it/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Indica se calcola tutte le formule ogni volta che viene avviato un calcolo.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Osservazioni

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante affinché altre applicazioni (come MS Excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni nella maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della formula
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Dimostra la proprietà ForceFullCalculation
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // Aggiungi dati di esempio e formula
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Calcola le formule con l'impostazione ForceFullCalculation
            workbook.CalculateFormula();

            // Restituisci il risultato
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // Salva la cartella di lavoro
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


