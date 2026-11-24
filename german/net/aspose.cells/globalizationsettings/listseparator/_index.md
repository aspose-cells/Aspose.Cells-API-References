---
title: "GlobalizationSettings.ListSeparator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GlobalizationSettings‑Eigenschaft. Gibt das Trennzeichen für Listenparameter einer Funktion …usw. zurück"
type: docs
url: /de/net/aspose.cells/globalizationsettings/listseparator/
---
## GlobalizationSettings.ListSeparator property

Liest das Trennzeichen für Listen, Funktionsparameter, ...usw.

```csharp
public virtual char ListSeparator { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit benutzerdefinierten Globalisierungseinstellungen
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zeige den aktuellen ListSeparator‑Wert aus unseren benutzerdefinierten Einstellungen an
            Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);

            // Erstelle eine Formel unter Verwendung des benutzerdefinierten ListSeparator
            worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
            worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";

            // Berechne Formeln mit benutzerdefiniertem Trennzeichen
            workbook.CalculateFormula();

            // Berechnungsergebnisse anzeigen
            Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);

            // Speichern mit Formeln unter Verwendung eines benutzerdefinierten Listentrennzeichens
            workbook.Save("ListSeparatorDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ListSeparator => ';';
        }
    }
}
```

### Siehe auch

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


