---
title: "FormulaSettings.CalculationMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Ottiene o imposta la modalità di calcolo della cartella di lavoro in MS Excel"
type: docs
url: /it/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

Ottiene o imposta la modalità di calcolo della cartella di lavoro in MS Excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Osservazioni

Questa proprietà serve solo per salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come MS Excel) possano comportarsi di conseguenza durante il caricamento e la manipolazione del file risultante. Per motivi di prestazioni nella maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dalla modalità impostata per questa proprietà. Se l'utente ha bisogno di calcolare le formule, si prega di chiamare sempre i metodi sugli oggetti appropriati secondo le esigenze: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...etc.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Imposta la modalità di calcolo su AutomaticExceptTable
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Cambia la modalità di calcolo su Manual
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Ripristina la modalità Automatic predefinita
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### Vedi anche

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


