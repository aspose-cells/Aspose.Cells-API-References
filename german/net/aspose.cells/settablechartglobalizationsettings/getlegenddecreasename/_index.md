---
title: "SettableChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Ruft den Namen der Verringerung für die Legende ab"
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/
---
## SettableChartGlobalizationSettings.GetLegendDecreaseName method

Liefert den Namen für 'Abnahme' in der Legende.

```csharp
public override string GetLegendDecreaseName()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einfache Daten für den Kontext hinzu (optional)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Erstellen Sie ein Diagramm (optional, nur um eine vollständige Arbeitsmappe zu haben)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Instanziiere das Globalisierungs‑Einstellungsobjekt.
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Legen Sie eine benutzerdefinierte Legenden‑Verringerungsbeschriftung fest
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Rufen Sie die Beschriftung mit GetLegendDecreaseName ab
                string legendDecreaseName = settings.GetLegendDecreaseName();

                Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

                // Speichere das Workbook (die Einstellungen sind in diesem Demo nicht direkt dem Diagramm zugeordnet).
                workbook.Save("GetLegendDecreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


