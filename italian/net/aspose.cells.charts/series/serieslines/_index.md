---
title: "Series.SeriesLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce un oggetto SeriesLines che rappresenta le linee di serie per un grafico a barre impilate o a colonne impilate. Si applica solo a grafici a barre impilate e a colonne impilate"
type: docs
url: /it/net/aspose.cells.charts/series/serieslines/
---
## Series.SeriesLines property

Restituisce un oggetto SeriesLines che rappresenta le linee di serie per un grafico a barre impilate o un grafico a colonne impilate. Si applica solo a grafici a barre impilate e a grafici a colonne impilate.

```csharp
public Line SeriesLines { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertySeriesLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["A5"].PutValue(4);
            
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Personalizza le linee di serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.SeriesLines.Color = Color.Red;
            series.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            
            // Salva la cartella di lavoro
            workbook.Save("SeriesLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


