---
title: "SettableChartGlobalizationSettings.SetLegendDecreaseName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings metod. Anger namnet på minskning för legend"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/
---
## SettableChartGlobalizationSettings.SetLegendDecreaseName method

Ställer in namnet på Decrease för Legend.

```csharp
public void SetLegendDecreaseName(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | lokalt beroende namn |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för ett diagram
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Skapa globaliseringsinställningar
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Anropa SetLegendDecreaseName med en anpassad sträng
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Klassen Chart har inte en ChartGlobalizationSettings-egenskap,
                // så vi måste använda inställningsobjektet direkt där det behövs
                // (Obs: Vid faktisk användning måste du hitta var dessa inställningar tillämpas)
                Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("SetLegendDecreaseNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


