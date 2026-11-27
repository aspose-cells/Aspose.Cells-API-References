---
title: "ChartGlobalizationSettings.GetChartTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings metod. Hämtar namnet på diagramtitel"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getcharttitlename/
---
## ChartGlobalizationSettings.GetChartTitleName method

Hämtar namnet på Chart Title.

```csharp
public virtual string GetChartTitleName()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetChartTitleNameDemo
    {
        public static void Run()
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

            // Demonstrera användningen av GetChartTitleName metoden
            string chartTitleName = globalizationSettings.GetChartTitleName();
            Console.WriteLine("Chart Title Name: " + chartTitleName);

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


