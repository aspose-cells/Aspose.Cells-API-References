---
title: "Chart.FilteredNSeries"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt eine SeriesCollection‑Sammlung zurück, die die Datenserien darstellt, die im Diagramm gefiltert sind"
type: docs
url: /de/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Gibt eine [`SeriesCollection`](../../seriescollection/)‑Sammlung zurück, die die Datenserien darstellt, die im Diagramm gefiltert sind.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu und setze einige Serien als gefiltert
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Einige Serien filtern (Serie 2 ausblenden)
            chart.NSeries[1].IsFiltered = true;

            // Auf gefilterte Serien‑Sammlung zugreifen
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // Speichere die Arbeitsmappe
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


