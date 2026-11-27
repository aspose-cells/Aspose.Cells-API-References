---
title: "Axis.IsPlotOrderReversed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis egenskap. Representerar om Microsoft Excel ritar datapunkter från sista till första"
type: docs
url: /sv/net/aspose.cells.charts/axis/isplotorderreversed/
---
## Axis.IsPlotOrderReversed property

Anger om Microsoft Excel ritar datapunkter från sista till första.

```csharp
public bool IsPlotOrderReversed { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsPlotOrderReversedDemo
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

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Omvänd ordning på diagrammets kategorier
            chart.CategoryAxis.IsPlotOrderReversed = true;

            // Spara arbetsboken
            workbook.Save("AxisPropertyIsPlotOrderReversedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


