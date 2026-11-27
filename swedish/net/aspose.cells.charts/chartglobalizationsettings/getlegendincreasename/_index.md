---
title: "ChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings metod. Hämtar namnet på ökning för legenden"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/
---
## ChartGlobalizationSettings.GetLegendIncreaseName method

Hämtar namnet på increase för Legend.

```csharp
public virtual string GetLegendIncreaseName()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett exempeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Skapa globaliseringsinställningar och hämta legenden ökningsnamn
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();

            // Skriv ut resultatet
            Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

            // Spara arbetsboken
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


