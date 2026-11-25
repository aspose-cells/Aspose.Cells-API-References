---
title: "Series.TrendLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce tutte le linee di tendenza di questa serie"
type: docs
url: /it/net/aspose.cells.charts/series/trendlines/
---
## Series.TrendLines property

Restituisce tutte le linee di tendenza di questa serie.

```csharp
public TrendlineCollection TrendLines { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyTrendLinesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Aggiungi una linea di tendenza esponenziale alla prima serie e ottienila per indice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;

            // Salva la cartella di lavoro
            workbook.Save("TrendLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


