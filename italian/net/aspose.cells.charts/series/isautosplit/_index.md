---
title: "Series.IsAutoSplit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Indica se il valore soglia è automatico"
type: docs
url: /it/net/aspose.cells.charts/series/isautosplit/
---
## Series.IsAutoSplit property

Indica se il valore soglia è automatico.

```csharp
public bool IsAutoSplit { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsAutoSplitDemo
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
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Accedi alla prima serie e dimostra la proprietà IsAutoSplit
            Series series = chart.NSeries[0];
            bool isAutoSplit = series.IsAutoSplit; // Get the value instead of setting it
            series.SplitValue = 25; // Split at value 25

            Console.WriteLine($"IsAutoSplit value: {isAutoSplit}");

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyIsAutoSplitDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


