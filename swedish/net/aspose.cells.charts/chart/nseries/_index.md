---
title: "Chart.NSeries"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Hämtar en SeriesCollection‑samling som representerar dataserierna i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Hämtar en [`SeriesCollection`](../../seriescollection/)‑samling som representerar dataserierna i diagrammet.

```csharp
public SeriesCollection NSeries { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNSeriesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // Ange datakällan för diagramserierna med NSeries
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // Ange diagramtitel
            chart.Title.Text = "NSeries Demo Chart";

            // Spara arbetsboken
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


