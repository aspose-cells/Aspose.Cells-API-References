---
title: "Series.DoughnutHoleSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Returnerar eller anger storleken på hålet i en donut‑diagramgrupp. Hålets storlek uttrycks som en procentsats av diagrammets storlek mellan 10 och 90 procent"
type: docs
url: /sv/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Returnerar eller anger storleken på hålet i en donutdiagramgrupp. Hålets storlek uttrycks som en procentsats av diagrammets storlek, mellan 10 och 90 procent.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till ett doughnut-diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in donut‑hålets storlek (procent av diagramradien)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // Spara arbetsboken
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


