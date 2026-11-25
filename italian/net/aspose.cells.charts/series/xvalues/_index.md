---
title: "Series.XValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Rappresenta i valori X di questa serie di grafico"
type: docs
url: /it/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Rappresenta i valori X di questa serie di grafico.

```csharp
public string XValues { get; set; }
```

### Osservazioni

Solo per i grafici Scatter e Bubble. Si prega di utilizzare [`CategoryData`](../../seriescollection/categorydata/) per altri tipi di grafici [`CategoryValues`](../categoryvalues/) è usato per ottenere i valori di categoria effettivi di questa serie.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // Aggiungi un grafico scatter
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi una serie con XValues e Values
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // Salva la cartella di lavoro
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


