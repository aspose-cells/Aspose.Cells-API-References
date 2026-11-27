---
title: "ChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings metod. Hämtar namnet på minskning för legenden"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/
---
## ChartGlobalizationSettings.GetLegendDecreaseName method

Hämtar namnet på Decrease för Legend.

```csharp
public virtual string GetLegendDecreaseName()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Skapa globaliseringsinställningar och hämta legenden minskningsnamn
            Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
            string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();

            // Skriv ut resultatet
            Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

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


