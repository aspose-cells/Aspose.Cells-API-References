---
title: "FormulaSettings.MaxIteration"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Il numero massimo di iterazioni per risolvere un riferimento circolare"
type: docs
url: /it/net/aspose.cells/formulasettings/maxiteration/
---
## FormulaSettings.MaxIteration property

Il numero massimo di iterazioni per risolvere un riferimento circolare.

```csharp
public int MaxIteration { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxIterationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 10;
            
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].Formula = "=A2+1";
            cells["A2"].Formula = "=A1+1";
            
            workbook.CalculateFormula();
            
            Console.WriteLine("A1 value: " + cells["A1"].Value);
            Console.WriteLine("A2 value: " + cells["A2"].Value);
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


