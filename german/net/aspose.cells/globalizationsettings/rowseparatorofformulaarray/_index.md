---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings‑Eigenschaft. Gibt das Trennzeichen für Zeilen in Array‑Daten in einer Formel zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

Liest das Trennzeichen für Zeilen in Array-Daten in einer Formel.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf die benutzerdefinierte Instanz der Globalisierungseinstellungen zu
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // Zeige den aktuellen Wert von RowSeparatorOfFormulaArray an
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Erstelle eine Array‑Formel unter Verwendung des benutzerdefinierten Zeilentrennzeichens
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // Berechne die Formel, um die korrekte Analyse zu demonstrieren
            workbook.CalculateFormula();

            // Ergebnisse anzeigen
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // Benutzerdefinierte GlobalizationSettings‑Implementierung, die das Zeilentrennzeichen überschreibt
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


