---
title: "Chart.NSeries"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene una collezione SeriesCollection che rappresenta le serie di dati nel grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Ottiene una collezione [`SeriesCollection`](../../seriescollection/) che rappresenta le serie di dati nel grafico.

```csharp
public SeriesCollection NSeries { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // Imposta l'origine dati per le serie del grafico usando NSeries
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // Imposta titolo del grafico
            chart.Title.Text = "NSeries Demo Chart";

            // Salva la cartella di lavoro
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


