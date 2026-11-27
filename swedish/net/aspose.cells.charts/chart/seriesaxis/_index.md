---
title: "Chart.SeriesAxis"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Hämtar diagrammets serieaxel"
type: docs
url: /sv/net/aspose.cells.charts/chart/seriesaxis/
---
## Chart.SeriesAxis property

Hämtar diagrammets serieaxel.

```csharp
public Axis SeriesAxis { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySeriesAxisDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Product B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Lägg till ett 3D-klustrat stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B1:C4", true);

            // Kom åt och konfigurera SeriesAxis
            Axis seriesAxis = chart.SeriesAxis;
            seriesAxis.Title.Text = "Product Series";
            seriesAxis.Title.Font.Size = 12;
            seriesAxis.Title.Font.IsBold = true;
            seriesAxis.MajorTickMark = TickMarkType.Cross;
            seriesAxis.MinorTickMark = TickMarkType.Outside;

            // Spara arbetsboken
            workbook.Save("ChartPropertySeriesAxisDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


