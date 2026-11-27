---
title: "Chart.FilteredNSeries"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Hämtar en SeriesCollection‑samling som representerar de dataserier som filtreras i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Hämtar en [`SeriesCollection`](../../seriescollection/)‑samling som representerar de dataserier som filtreras i diagrammet.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFilteredNSeriesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram och markera vissa serier som filtrerade
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Filtrera vissa serier (dölj Serie 2)
            chart.NSeries[1].IsFiltered = true;

            // Åtkomst till filtrerad seriekollektion
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // Spara arbetsboken
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


