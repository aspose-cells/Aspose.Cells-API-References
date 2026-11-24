---
title: "FormulaSettings.ForceFullCalculation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln berechnet werden."
type: docs
url: /de/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Hinweise

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellendatei, damit andere Anwendungen (wie MS Excel) beim Laden und Bearbeiten der Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formeln in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf die Formeleinstellungen zugreifen
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // ForceFullCalculation-Eigenschaft demonstrieren
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // Beispieldaten und Formel hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Formeln mit der Einstellung ForceFullCalculation berechnen
            workbook.CalculateFormula();

            // Gib das Ergebnis aus
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // Speichere die Arbeitsmappe
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


