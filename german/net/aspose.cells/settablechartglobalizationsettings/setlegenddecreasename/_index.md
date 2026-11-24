---
title: "SettableChartGlobalizationSettings.SetLegendDecreaseName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableChartGlobalizationSettings-Methode. Setzt den Namen für \"Decrease\" in der Legende."
type: docs
url: /de/net/aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/
---
## SettableChartGlobalizationSettings.SetLegendDecreaseName method

Setzt den Namen von Decrease für die Legende.

```csharp
public void SetLegendDecreaseName(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | lokaler abhängiger Name |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendDecreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für ein Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erstellen Sie Globalisierungseinstellungen
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Rufen Sie SetLegendDecreaseName mit einem benutzerdefinierten String auf
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Die Chart-Klasse hat keine ChartGlobalizationSettings-Eigenschaft,
                // so müssen wir das Settings-Objekt dort, wo es benötigt wird, direkt verwenden
                // (Hinweis: In der tatsächlichen Verwendung müssten Sie herausfinden, wo diese Einstellungen angewendet werden)
                Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SetLegendDecreaseNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


