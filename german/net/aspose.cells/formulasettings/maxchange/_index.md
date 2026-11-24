---
title: "FormulaSettings.MaxChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Die maximale Änderung, um einen zirkulären Verweis aufzulösen"
type: docs
url: /de/net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

Die maximale Änderung, um eine zirkuläre Referenz zu lösen.

```csharp
public double MaxChange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyMaxChangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Richten Sie die Einstellungen für die iterative Berechnung ein
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Settings.FormulaSettings.MaxChange = 0.001; // Set maximum change threshold
            
            // Erstellen Sie einen zirkulären Verweis für die Demonstration
            worksheet.Cells["A1"].Formula = "=B1+1";
            worksheet.Cells["B1"].Formula = "=A1+1";
            
            // Berechnen Sie Formeln mit der angegebenen MaxChange-Einstellung
            workbook.CalculateFormula();
            
            // Ergebnisse ausgeben
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("MaxChange used: " + workbook.Settings.FormulaSettings.MaxChange);
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


