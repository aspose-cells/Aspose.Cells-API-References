---
title: "Series.SecondPlotSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà della serie. Restituisce o imposta la dimensione della sezione secondaria di un grafico a torta di torta o di un grafico a barra di torta come percentuale della dimensione della torta primaria. Può essere un valore da 5 a 200"
type: docs
url: /it/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

Restituisce o imposta la dimensione della sezione secondaria di un grafico a torta di torta o di un grafico a barra di torta, come percentuale della dimensione della torta primaria. Può essere un valore da 5 a 200.

```csharp
public short SecondPlotSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a torta
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie
            Series series = chart.NSeries[0];

            // Imposta la proprietà SecondPlotSize (percentuale della torta da mostrare nel secondo grafico)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


