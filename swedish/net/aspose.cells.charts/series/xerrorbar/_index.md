---
title: "Series.XErrorBar"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Representerar felstapeln i X‑riktning för serien."
type: docs
url: /sv/net/aspose.cells.charts/series/xerrorbar/
---
## Series.XErrorBar property

Representerar X‑riktningens felstapel för serien.

```csharp
public ErrorBar XErrorBar { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXErrorBarDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serie med data
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            Series series = seriesCollection[0];
            series.XValues = "A2:A4";

            // Konfigurera XErrorBar-egenskaper
            series.XErrorBar.DisplayType = ErrorBarDisplayType.Plus;
            series.XErrorBar.Amount = 0.5;
            series.XErrorBar.Type = ErrorBarType.FixedValue;

            // Spara arbetsboken
            workbook.Save("SeriesPropertyXErrorBarDemo.xlsx");
        }
    }
}
```

### Se även

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


