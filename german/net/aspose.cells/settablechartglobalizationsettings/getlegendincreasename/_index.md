---
title: "SettableChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Gibt den Namen der Erhöhung für die Legende zurück."
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

Liefert den Namen für 'Zunahme' in der Legende.

```csharp
public override string GetLegendIncreaseName()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
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

                // Legen Sie einen benutzerdefinierten Legenden‑Erhöhungsnamen fest
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Rufen Sie den Namen der Legenden‑Erhöhung mit GetLegendIncreaseName ab.
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

                // Speichere die Arbeitsmappe
                workbook.Save("GetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


