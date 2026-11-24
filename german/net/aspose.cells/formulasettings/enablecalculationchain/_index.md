---
title: "FormulaSettings.EnableCalculationChain"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. Standard ist false."
type: docs
url: /de/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. Standard ist false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Hinweise

Wenn sich viele Formeln in der Arbeitsmappe befinden und der Benutzer sie wiederholt berechnen muss, wobei nur ein kleiner Teil davon geändert wird, kann das Aktivieren der Berechnungskette aus Leistungsgründen hilfreich sein. Auf der anderen Seite erfordert die Aufrechterhaltung des Kettenmodells bei aktivierter Kette zusätzlichen Speicher und verbraucht etwas mehr CPU‑Zeit für andere Vorgänge, wie das Ändern des Zellwerts oder von Formeln. Nachdem diese Eigenschaft von false auf true geändert wurde, wird die Berechnungskette beim ersten Berechnen der Arbeitsmappe analysiert und aufgebaut, sodass die für die erste Berechnung benötigte Zeit länger sein kann als bei einer normalen Berechnung ohne Kette.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispiel-Formeln hinzufügen
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // Berechnungskette deaktivieren
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // Formeln berechnen
            workbook.CalculateFormula();
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


