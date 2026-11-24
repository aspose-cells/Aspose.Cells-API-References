---
title: "SettablePivotGlobalizationSettings.SetTextOfColumnLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettablePivotGlobalizationSettings-Methode. Gibt den Text der Beschriftung \"Column Labels\" in der PivotTable zurück"
type: docs
url: /de/net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

Ermittelt den Text der Beschriftung "Column Labels" in der PivotTable.

```csharp
public void SetTextOfColumnLabels(string text)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text der Spaltenbeschriftungen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe (nur zum Kontext)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Erstelle eine Instanz von SettablePivotGlobalizationSettings
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // Lege benutzerdefinierten Text für die Beschriftung "Column Labels" fest
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // Rufe den aktuellen Text ab, um die Änderung zu überprüfen
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // Speichere die Arbeitsmappe (für diese Demo ist keine Pivot-Tabelle erforderlich)
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


