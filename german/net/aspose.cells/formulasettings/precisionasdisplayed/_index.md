---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt an, ob die Genauigkeit des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird"
type: docs
url: /de/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Gibt an, ob die Genauigkeit des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Setzen Sie PrecisionAsDisplayed auf true
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Legen Sie das Anzeigeformat für Zelle A1 fest, um 2 Dezimalstellen anzuzeigen
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // Setzen Sie die Formel in B1, die sich auf A1 bezieht
            cells["B1"].Formula = "=A1";
            
            // Berechnen Sie Formeln mit aktivierter PrecisionAsDisplayed
            workbook.CalculateFormula();
            
            // Ergebnisse ausgeben
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


