---
title: "Chart.FilteredNSeries"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene una collezione SeriesCollection che rappresenta le serie di dati filtrate nel grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Ottiene una collezione [`SeriesCollection`](../../seriescollection/) che rappresenta le serie di dati filtrate nel grafico.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico e imposta alcune serie come filtrate
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Filtra alcune serie (nascondi Serie 2)
            chart.NSeries[1].IsFiltered = true;

            // Accedi alla collezione di serie filtrate
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // Salva la cartella di lavoro
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


