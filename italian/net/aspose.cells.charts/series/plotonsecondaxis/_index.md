---
title: "Series.PlotOnSecondAxis"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Indica se questa serie è tracciata sul secondo asse dei valori"
type: docs
url: /it/net/aspose.cells.charts/series/plotonsecondaxis/
---
## Series.PlotOnSecondAxis property

Indica se questa serie è tracciata sul secondo asse dei valori.

```csharp
public bool PlotOnSecondAxis { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyPlotOnSecondAxisDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la prima serie per essere tracciata sull'asse secondario
            chart.NSeries[0].PlotOnSecondAxis = true;

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyPlotOnSecondAxisDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


