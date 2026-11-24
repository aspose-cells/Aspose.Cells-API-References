---
title: "FormulaSettings.EnableIterativeCalculation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt an, ob die iterative Berechnung aktiviert werden soll, um zirkuläre Verweise aufzulösen"
type: docs
url: /de/net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Gibt an, ob die iterative Berechnung aktiviert werden soll, um zirkuläre Verweise zu lösen.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableIterativeCalculationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Richten Sie einen zirkulären Verweis für die Demonstration ein
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Aktivieren Sie die iterative Berechnung mit maximalen Durchläufen
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001;
            
            // Formeln berechnen
            workbook.CalculateFormula();
            
            // Ergebnisse ausgeben
            Console.WriteLine("A1 value after calculation: " + worksheet.Cells["A1"].DoubleValue);
            Console.WriteLine("B1 value after calculation: " + worksheet.Cells["B1"].DoubleValue);
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


