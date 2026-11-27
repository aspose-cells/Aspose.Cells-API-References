---
title: "Klass SettableChartGlobalizationSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SettableChartGlobalizationSettings-klass. Implementation av PivotGlobalizationSettings som möjliggör för användaren att ange/ändra fördefinierade texter"
type: docs
url: /sv/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

Implementering av PivotGlobalizationSettings som låter användaren ange/ändra fördefinierade texter.

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Hämtar namnet på Title för Axis. |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Hämtar namnet på Axis Unit. |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Hämtar namnet på Chart Title. |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Hämtar namnet på Decrease för Legend. |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Hämtar namnet på increase för Legend. |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Hämtar namnet på Total för Legend. |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Hämtar namnet på "Other"-etiketter för Chart. |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Hämtar namnet på Series i Chart. |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Ställer in namnet på Title för Axis. |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Ställer in namnet på Axis Unit. |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Ställer in namnet på Chart Title. |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Ställer in namnet på Decrease för Legend. |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Ställer in namnet på increase för Legend. |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Ställer in namnet på Total för Legend. |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Ställer in namnet på "Other"-etiketter för Chart. |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Ställer in namnet på Series i Chart. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CellsClassSettableChartGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en instans av SettableChartGlobalizationSettings
                var settings = new SettableChartGlobalizationSettings();

                // Ställ in anpassade globaliseringsinställningar
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // Skapa en anpassad GlobalizationSettings-implementation
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // Skapa ett enkelt diagram för att demonstrera inställningarna
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Q1");
                worksheet.Cells["A3"].PutValue("Q2");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);

                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";
                chart.Title.Text = "Demo Chart";

                Console.WriteLine("SettableChartGlobalizationSettings configured successfully");
                workbook.Save("SettableChartGlobalizationSettingsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SettableChartGlobalizationSettings: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            private readonly SettableChartGlobalizationSettings _chartSettings;

            public CustomGlobalizationSettings(SettableChartGlobalizationSettings chartSettings)
            {
                _chartSettings = chartSettings;
            }

            // Implementera erforderliga GlobalizationSettings-metoder här
            // som delegerar till SettableChartGlobalizationSettings-instansen
        }
    }
}
```

### Se även

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


