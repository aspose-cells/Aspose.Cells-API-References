---
title: "FormulaSettings.MaxChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. La variazione massima per risolvere un riferimento circolare"
type: docs
url: /it/net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

La variazione massima per risolvere un riferimento circolare.

```csharp
public double MaxChange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxChangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configura le impostazioni di calcolo iterativo
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
            
            // Crea un riferimento circolare per dimostrazione
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Calcola le formule con l'impostazione MaxChange specificata
            workbook.CalculateFormula();
            
            // Restituisci i risultati
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


