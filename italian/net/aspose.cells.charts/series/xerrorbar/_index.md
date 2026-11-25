---
title: "Series.XErrorBar"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Rappresenta la barra di errore in direzione X della serie"
type: docs
url: /it/net/aspose.cells.charts/series/xerrorbar/
---
## Series.XErrorBar property

Rappresenta la barra di errore in direzione X della serie.

```csharp
public ErrorBar XErrorBar { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi la serie usando i dati
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            Series series = seriesCollection[0];
            series.XValues = "A2:A4";

            // Configura le proprietà XErrorBar
            series.XErrorBar.DisplayType = ErrorBarDisplayType.Plus;
            series.XErrorBar.Amount = 0.5;
            series.XErrorBar.Type = ErrorBarType.FixedValue;

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyXErrorBarDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


