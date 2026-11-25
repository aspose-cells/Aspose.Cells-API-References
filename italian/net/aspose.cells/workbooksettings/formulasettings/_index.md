---
title: "WorkbookSettings.FormulaSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene le impostazioni per le funzionalità correlate alle formule"
type: docs
url: /it/net/aspose.cells/workbooksettings/formulasettings/
---
## WorkbookSettings.FormulaSettings property

Ottiene le impostazioni per le funzionalità relative alle formule.

```csharp
public FormulaSettings FormulaSettings { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFormulaSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi e modifica FormulaSettings
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;

            // Visualizza le impostazioni
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
            Console.WriteLine("Iterative Calculation Enabled: " + workbook.Settings.FormulaSettings.EnableIterativeCalculation);
            Console.WriteLine("Max Iterations: " + workbook.Settings.FormulaSettings.MaxIteration);
            Console.WriteLine("Max Change: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


