---
title: "Klasse FormulaSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FormulaSettings-Klasse. Einstellungen für Formeln und Berechnungen"
type: docs
url: /de/net/aspose.cells/formulasettings/
---
## FormulaSettings class

Einstellungen für Formeln und Berechnungen.

```csharp
public class FormulaSettings
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Gibt die Version der Berechnungs-Engine an, die zum Berechnen von Werten in der Arbeitsmappe verwendet wird. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | Liefert oder setzt den Modus für die Arbeitsmappenberechnung in MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. Standard ist false. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Gibt an, ob die iterative Berechnung aktiviert werden soll, um zirkuläre Verweise zu lösen. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | Die maximale Änderung, um eine zirkuläre Referenz zu lösen. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | Die maximale Anzahl an Iterationen, um eine zirkuläre Referenz zu lösen. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Gibt an, ob die Genauigkeit des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt werden, beim Abrufen und Setzen von Formeln erhalten bleiben sollen. Der Standardwert ist false. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf die Formeleinstellungen der Arbeitsmappe
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Eigenschaften festlegen
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Speichere die Arbeitsmappe
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


