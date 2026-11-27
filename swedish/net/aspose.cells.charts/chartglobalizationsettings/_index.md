---
title: "Klass ChartGlobalizationSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartGlobalizationSettings-klass. Representerar globaliseringsinställningarna för ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/
---
## ChartGlobalizationSettings class

Representerar globaliseringsinställningarna för ett diagram.

```csharp
public class ChartGlobalizationSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ChartGlobalizationSettings](chartglobalizationsettings/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [GetAxisTitleName](../../aspose.cells.charts/chartglobalizationsettings/getaxistitlename/)() | Hämtar namnet på Title för Axis. |
| virtual [GetAxisUnitName](../../aspose.cells.charts/chartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Hämtar namnet på Axis Unit. |
| virtual [GetChartTitleName](../../aspose.cells.charts/chartglobalizationsettings/getcharttitlename/)() | Hämtar namnet på Chart Title. |
| virtual [GetLegendDecreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/)() | Hämtar namnet på Decrease för Legend. |
| virtual [GetLegendIncreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/)() | Hämtar namnet på increase för Legend. |
| virtual [GetLegendTotalName](../../aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/)() | Hämtar namnet på Total för Legend. |
| virtual [GetOtherName](../../aspose.cells.charts/chartglobalizationsettings/getothername/)() | Hämtar namnet på "Other"-etiketter för Chart. |
| virtual [GetSeriesName](../../aspose.cells.charts/chartglobalizationsettings/getseriesname/)() | Hämtar namnet på Series i Chart. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartGlobalizationSettingsDemo
    {
        public static void ChartGlobalizationSettingsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett exempeldiagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Skapa en instans av ChartGlobalizationSettings
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();

            // Demonstrera användningen av metoder i ChartGlobalizationSettings
            string seriesName = globalizationSettings.GetSeriesName();
            string chartTitleName = globalizationSettings.GetChartTitleName();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
            string legendTotalName = globalizationSettings.GetLegendTotalName();
            string axisTitleName = globalizationSettings.GetAxisTitleName();
            string otherName = globalizationSettings.GetOtherName();
            string axisUnitName = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);

            // Skriv ut de hämtade namnen till konsolen
            Console.WriteLine("Series Name: " + seriesName);
            Console.WriteLine("Chart Title Name: " + chartTitleName);
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
            Console.WriteLine("Legend Total Name: " + legendTotalName);
            Console.WriteLine("Axis Title Name: " + axisTitleName);
            Console.WriteLine("Other Name: " + otherName);
            Console.WriteLine("Axis Unit Name: " + axisUnitName);

            // Spara arbetsboken
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
            workbook.Save("ChartGlobalizationSettingsExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


