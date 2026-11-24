---
title: "FormulaSettings.MaxIteration"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Die maximale Anzahl von Durchläufen, um eine zirkuläre Referenz aufzulösen."
type: docs
url: /de/net/aspose.cells/formulasettings/maxiteration/
---
## FormulaSettings.MaxIteration property

Die maximale Anzahl an Iterationen, um eine zirkuläre Referenz zu lösen.

```csharp
public int MaxIteration { get; set; }
```

### Beispiele

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

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


