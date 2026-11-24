---
title: "SettableChartGlobalizationSettings.SetSeriesName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Legt den Namen der Serie im Diagramm fest"
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/setseriesname/
---
## SettableChartGlobalizationSettings.SetSeriesName method

Setzt den Namen der Serie im Diagramm.

```csharp
public void SetSeriesName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetSeriesNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie minimale Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Erstelle eine Instanz von SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Setzen Sie einen benutzerdefinierten Seriennamen mit SetSeriesName und einem String-Parameter.
                settings.SetSeriesName("Custom Series Label");

                // Überprüfen Sie die Einstellung, indem Sie den Seriennamen abrufen.
                string seriesName = settings.GetSeriesName();
                Console.WriteLine($"Series name set to: {seriesName}");

                // Speichere die Arbeitsmappe
                workbook.Save("SetSeriesNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetSeriesName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


