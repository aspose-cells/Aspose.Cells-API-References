---
title: "SettablePivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Gibt den Text der \"Row Labels\"‑Beschriftung in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/gettextofrowlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfRowLabels method

Ermittelt den Text der Beschriftung "Row Labels" in der PivotTable.

```csharp
public override string GetTextOfRowLabels()
```

### Rückgabewert

Der Text der Zeilenbeschriftungen

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Beispieldaten zum Kontext hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Erstelle eine Instanz von SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Benutzerdefinierten Text für Zeilenbeschriftungen festlegen
                settings.SetTextOfRowLabels("Custom Row Labels");

                // Den Text der Zeilenbeschriftungen abrufen
                string rowLabelsText = settings.GetTextOfRowLabels();

                Console.WriteLine($"Text of Row Labels: {rowLabelsText}");

                // Speichere die Arbeitsmappe
                workbook.Save("GetTextOfRowLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


