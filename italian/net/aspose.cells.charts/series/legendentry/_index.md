---
title: "Series.LegendEntry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene la voce della legenda corrispondente a questa serie"
type: docs
url: /it/net/aspose.cells.charts/series/legendentry/
---
## Series.LegendEntry property

Ottiene la voce della legenda corrispondente a questa serie.

```csharp
public LegendEntry LegendEntry { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLegendEntryDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie
            Series series = chart.NSeries[0];

            // Dimostra la funzionalità di LegendEntry
            Console.WriteLine("LegendEntry.IsDeleted before: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = true;
            Console.WriteLine("LegendEntry.IsDeleted after setting to true: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = false;
            Console.WriteLine("LegendEntry.IsDeleted after setting to false: " + series.LegendEntry.IsDeleted);

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyLegendEntryDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


