---
title: "SettableChartGlobalizationSettings.SetLegendTotalName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Setzt den Namen des Gesamts für die Legende fest."
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/setlegendtotalname/
---
## SettableChartGlobalizationSettings.SetLegendTotalName method

Setzt den Namen von Total für die Legende.

```csharp
public void SetLegendTotalName(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | lokaler abhängiger Name |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendTotalNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie minimale Daten für den Kontext hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Erstelle eine Instanz von SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Setzen Sie einen benutzerdefinierten Gesamtnamen für die Legende.
                settings.SetLegendTotalName("Custom Total Label");

                // Überprüfen Sie die Einstellung, indem Sie den Wert abrufen
                string legendTotalName = settings.GetLegendTotalName();
                Console.WriteLine("Legend Total Name set to: " + legendTotalName);

                // Speichere die Arbeitsmappe
                workbook.Save("SetLegendTotalNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


