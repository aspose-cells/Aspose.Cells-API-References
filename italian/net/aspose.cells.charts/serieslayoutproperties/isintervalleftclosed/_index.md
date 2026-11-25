---
title: "SeriesLayoutProperties.IsIntervalLeftClosed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesLayoutProperties. Indica se l'intervallo è chiuso sul lato sinistro"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/
---
## SeriesLayoutProperties.IsIntervalLeftClosed property

Indica se l'intervallo è chiuso sul lato sinistro.

```csharp
public bool IsIntervalLeftClosed { get; set; }
```

### Osservazioni

Solo per il grafico ParetoLine.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyIsIntervalLeftClosedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];

            // Imposta la proprietà IsIntervalLeftClosed
            series.LayoutProperties.IsIntervalLeftClosed = true;

            // Salva cartella di lavoro
            workbook.Save("SeriesLayoutPropertiesIsIntervalLeftClosedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


