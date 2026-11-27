---
title: "Series.FirstSliceAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Hämtar eller anger vinkeln för den första piechart‑ eller doughnutchart‑sektorn i grader medurs från vertikal. Gäller endast pie‑, 3D‑pie‑ och doughnut‑diagram med värden från 0 till 360"
type: docs
url: /sv/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

Hämtar eller anger vinkeln för den första paj- eller donutskivan, i grader (medurs från vertikal). Gäller endast för paj-, 3‑D-paj- och donutdiagram, med värden från 0 till 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pajdiagram
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första serien och ange FirstSliceAngle
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


