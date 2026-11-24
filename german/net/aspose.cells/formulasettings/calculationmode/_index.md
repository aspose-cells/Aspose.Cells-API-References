---
title: "FormulaSettings.CalculationMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormulaSettings-Eigenschaft. Ruft den Modus für die Arbeitsmappenberechnung in MS Excel ab oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

Liefert oder setzt den Modus für die Arbeitsmappenberechnung in MS Excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Hinweise

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellendatei, damit andere Anwendungen (wie MS Excel) beim Laden und Verarbeiten der Datei entsprechend reagieren können. Aus Performance-Gründen für die meisten Benutzeranwendungen berechnen wir keine Formeln in der Arbeitsmappe automatisch, unabhängig davon, welcher Modus für diese Eigenschaft festgelegt wurde. Wenn der Benutzer Formeln berechnen muss, rufen Sie bitte stets die Methoden auf den jeweiligen Objekten gemäß den Anforderungen auf: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...etc.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Setzen Sie den Berechnungsmodus auf AutomaticExceptTable
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Ändern Sie den Berechnungsmodus zu Manual
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Zurücksetzen auf den Standardmodus Automatic
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### Siehe auch

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


