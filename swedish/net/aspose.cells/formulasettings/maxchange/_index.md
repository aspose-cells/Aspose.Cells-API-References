---
title: "FormulaSettings.MaxChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Den maximala förändringen för att lösa en cirkulär referens"
type: docs
url: /sv/net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

Den maximala förändringen för att lösa en cirkulär referens.

```csharp
public double MaxChange { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxChangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in iterativa beräkningsinställningar
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
            
            // Skapa en cirkulär referens för demonstration
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Beräkna formler med den angivna MaxChange-inställningen
            workbook.CalculateFormula();
            
            // Skriv ut resultat
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


