---
title: "DataLabels.ShowSeriesName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Anger om serienamnet visas på dataetiketterna i ett diagram. True för att visa serienamnet. False för att dölja"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Anger om seriens namn visas på dataetiketterna i ett diagram. True för att visa seriens namn. False för att dölja.

```csharp
public bool ShowSeriesName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // Aktivera dataetiketter för den första serien
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Aktivera visning av serienamn för specifik punkts dataetikett
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // Beräkna diagrammet
            chart.Calculate();

            // Spara arbetsboken
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


