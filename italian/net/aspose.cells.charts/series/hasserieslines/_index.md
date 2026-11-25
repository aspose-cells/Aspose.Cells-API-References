---
title: "Series.HasSeriesLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. True se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. Si applica solo a grafici a colonne impilate, grafici a barre, grafici Pie of Pie o Bar of Pie"
type: docs
url: /it/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

Vero se un grafico a colonne impilate o a barre ha linee di serie o se un grafico Pie of Pie o Bar of Pie ha linee di collegamento tra le due sezioni. Si applica solo a grafici a colonne impilate, a barre, Pie of Pie o Bar of Pie.

```csharp
public bool HasSeriesLines { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Aggiungi un grafico a colonne impilate
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi dati della serie
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Accedi alla prima serie
            Series series = chart.NSeries[0];
            
            // Dimostra la proprietà HasSeriesLines
            series.HasSeriesLines = true; // Enable series lines
            
            // Salva la cartella di lavoro
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


