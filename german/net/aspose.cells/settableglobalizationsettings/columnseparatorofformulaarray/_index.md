---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings‑Eigenschaft. Gibt das Trennzeichen für die Elemente in Zeilendaten von Arrays in einer Formel zurück."
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

Liest das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in einer Formel.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Zeigen Sie den aktuellen Wert von ColumnSeparatorOfFormulaArray an.
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // Setzen Sie einen neuen Wert für ColumnSeparatorOfFormulaArray.
            settings.SetColumnSeparatorOfFormulaArray(';');

            // Wenden Sie die Einstellungen auf die Arbeitsmappe an.
            workbook.Settings.GlobalizationSettings = settings;

            // Erstellen Sie eine Array‑Formel mit dem benutzerdefinierten Trennzeichen mittels SetArrayFormula.
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // Formeln berechnen
            workbook.CalculateFormula();

            // Ergebnis anzeigen
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


