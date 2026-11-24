---
title: "SettableChartGlobalizationSettings.GetLegendTotalName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Gibt den Namen des Totals für die Legende zurück"
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

Ermittelt den Namen von Total für die Legende.

```csharp
public override string GetLegendTotalName()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Erstelle eine Instanz von SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Setzen Sie zunächst einen benutzerdefinierten Legendentotalnamen
                settings.SetLegendTotalName("Custom Total Label");

                // Rufen Sie die GetLegendTotalName-Methode auf, um den Wert abzurufen
                string legendTotalName = settings.GetLegendTotalName();

                // Ergebnis anzeigen
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // Speichere die Arbeitsmappe
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


