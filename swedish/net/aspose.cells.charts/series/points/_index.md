---
title: "Series.Points"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Hämtar samlingen av punkter i en serie i ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/series/points/
---
## Series.Points property

Hämtar samlingen av punkter i en serie i ett diagram.

```csharp
public ChartPointCollection Points { get; }
```

### Anmärkningar

När diagrammet är Pie of Pie eller Bar of Pie är den sista punkten en annan punkt i den första pajdiagrammet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPointsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Kom åt den första serien och dess punkter
            Series series = chart.NSeries[0];
            foreach (ChartPoint point in series.Points)
            {
                // Lägg till datamärkningar till varje punkt
                point.DataLabels.ShowValue = true;
                point.DataLabels.ShowCellRange = true;
            }

            // Spara arbetsboken
            workbook.Save("SeriesPropertyPointsDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


