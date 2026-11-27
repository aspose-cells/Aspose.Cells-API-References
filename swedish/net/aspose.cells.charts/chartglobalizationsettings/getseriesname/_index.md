---
title: "ChartGlobalizationSettings.GetSeriesName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings-metod. Hämtar namnet på serier i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getseriesname/
---
## ChartGlobalizationSettings.GetSeriesName method

Hämtar namnet på Series i Chart.

```csharp
public virtual string GetSeriesName()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till ett diagram och ange data
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Skapa globaliseringsinställningar och hämta seriens namn
            Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
            string seriesName = globalizationSettings.GetSeriesName();

            // Skriv ut resultatet
            Console.WriteLine("Series Name: " + seriesName);

            // Spara arbetsboken
            workbook.Save("ChartGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### Se även

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


