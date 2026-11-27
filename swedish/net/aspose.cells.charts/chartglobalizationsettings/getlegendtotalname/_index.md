---
title: "ChartGlobalizationSettings.GetLegendTotalName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartGlobalizationSettings metod. Hämtar namnet på totalen för legenden"
type: docs
url: /sv/net/aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/
---
## ChartGlobalizationSettings.GetLegendTotalName method

Hämtar namnet på Total för Legend.

```csharp
public virtual string GetLegendTotalName()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartGlobalizationSettingsMethodGetLegendTotalNameDemo
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

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Skapa globaliseringsinställningar och hämta legenden totala namn
            ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
            string legendTotalName = globalizationSettings.GetLegendTotalName();

            // Skriv ut resultatet
            Console.WriteLine("Legend Total Name: " + legendTotalName);

            // Spara arbetsbok
            workbook.Save("ChartGlobalizationDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


