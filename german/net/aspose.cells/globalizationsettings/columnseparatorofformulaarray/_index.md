---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings-Eigenschaft. Gibt das Trennzeichen für die Elemente in Zeilendaten von Arrays in Formeln zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

Liest das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in einer Formel.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle benutzerdefinierte Globalisierungseinstellungen mit überschriebenem Spaltentrennzeichen
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Zeige den aktuellen Wert des Spaltentrennzeichens an
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // Erstelle Array-Formel mit benutzerdefiniertem Trennzeichen
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // Überprüfe die Formelablage (zeigt in der tatsächlichen Formelzeichenkette Semikolons an)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


