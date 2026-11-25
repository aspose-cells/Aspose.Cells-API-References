---
title: "FormulaSettings.EnableIterativeCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Indica se abilitare il calcolo iterativo per risolvere riferimenti circolari"
type: docs
url: /it/net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Indica se abilitare il calcolo iterativo per risolvere riferimenti circolari.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableIterativeCalculationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configura un riferimento circolare per la dimostrazione
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Abilita il calcolo iterativo con il numero massimo di iterazioni
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;
            
            // Calcola le formule
            workbook.CalculateFormula();
            
            // Restituisci i risultati
            Console.WriteLine("A1 value after calculation: " + worksheet.Cells["A1"].DoubleValue);
            Console.WriteLine("B1 value after calculation: " + worksheet.Cells["B1"].DoubleValue);
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


