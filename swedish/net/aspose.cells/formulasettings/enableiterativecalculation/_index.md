---
title: "FormulaSettings.EnableIterativeCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser"
type: docs
url: /sv/net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableIterativeCalculationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en cirkulär referens för demonstration
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Aktivera iterativ beräkning med maximalt antal iterationer
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;
            
            // Beräkna formler
            workbook.CalculateFormula();
            
            // Skriv ut resultat
            Console.WriteLine("A1 value after calculation: " + worksheet.Cells["A1"].DoubleValue);
            Console.WriteLine("B1 value after calculation: " + worksheet.Cells["B1"].DoubleValue);
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


