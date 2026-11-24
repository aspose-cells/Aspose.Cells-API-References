---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Eigenschaft. Gibt das Trennzeichen für Zeilen in Arraydaten in Formeln zurück"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

Liest das Trennzeichen für Zeilen in Array-Daten in einer Formel.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Zeigen Sie das Standardzeilentrennzeichen für Formel-Arrays an
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Legen Sie ein neues Zeilentrennzeichen für Formel-Arrays fest
            settings.SetRowSeparatorOfFormulaArray(';');

            // Wenden Sie die Einstellungen auf die Arbeitsmappe an
            workbook.Settings.GlobalizationSettings = settings;

            // Erstelle eine Array-Formel im Arbeitsblatt
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // Formeln berechnen
            workbook.CalculateFormula();

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


