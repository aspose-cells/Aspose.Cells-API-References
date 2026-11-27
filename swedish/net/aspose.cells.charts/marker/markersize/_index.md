---
title: "Marker.MarkerSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Marker-egenskap. Representerar markörens storlek i enheten punkter. Gäller för linjediagram, spridningsdiagram eller radardiagram"
type: docs
url: /sv/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Representerar markörens storlek i enheter av punkter. Gäller för linjediagram, spridningsdiagram eller radardiagram.

```csharp
public int MarkerSize { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier - korrigerat metodanrop
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // Ställ in markörens egenskaper
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // Spara arbetsboken
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


