---
title: "Series.DoughnutHoleSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà della serie. Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. La dimensione del foro è espressa come percentuale della dimensione del grafico tra il 10% e il 90%"
type: docs
url: /it/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Restituisce o imposta la dimensione del foro in un gruppo di grafico a ciambella. La dimensione del foro è espressa come percentuale della dimensione del grafico, tra il 10 e il 90 percento.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi un grafico a ciambella
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la dimensione del foro della ciambella (percentuale del raggio del grafico)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // Salva la cartella di lavoro
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


