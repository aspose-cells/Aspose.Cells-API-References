---
title: "Series.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce o imposta un tipo di serie dati"
type: docs
url: /it/net/aspose.cells.charts/series/type/
---
## Series.Type property

Ottiene o imposta il tipo di una serie di dati.

```csharp
public ChartType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyTypeDemo
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

            // Aggiungi un grafico a colonne impilate
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Verifica e stampa il tipo di serie
            foreach (Series series in chart.NSeries)
            {
                Console.WriteLine("Series Type: " + series.Type);
            }
        }
    }
}
```

### Vedi anche

* enum [ChartType](../../charttype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


