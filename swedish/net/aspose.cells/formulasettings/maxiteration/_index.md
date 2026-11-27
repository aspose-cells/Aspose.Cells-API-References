---
title: "FormulaSettings.MaxIteration"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskapen. Det maximala antalet iterationer för att lösa en cirkulär referens"
type: docs
url: /sv/net/aspose.cells/formulasettings/maxiteration/
---
## FormulaSettings.MaxIteration property

Det maximala antalet iterationer för att lösa en cirkulär referens.

```csharp
public int MaxIteration { get; set; }
```

### Exempel

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

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


