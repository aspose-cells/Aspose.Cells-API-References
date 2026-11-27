---
title: "SettableChartGlobalizationSettings.GetSeriesName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableChartGlobalizationSettings‑metod. Hämtar namnet på Series i Chart"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/getseriesname/
---
## SettableChartGlobalizationSettings.GetSeriesName method

Hämtar namnet på Series i Chart.

```csharp
public override string GetSeriesName()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Column A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Column B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Skapa och tillämpa globaliseringsinställningar
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetSeriesName("Custom Series Name");
            
            // Globaliseringsinställningarna används vid rendering/visning av chart,
            // men inte direkt tilldelade chart‑objektet
            // (eftersom Chart‑klassen inte har denna egenskap)

            try
            {
                // Hämta det anpassade serienamnet
                string seriesName = settings.GetSeriesName();
                Console.WriteLine("Series Name: " + seriesName);

                // Spara arbetsboken
                workbook.Save("MethodGetSeriesNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesName method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


