---
title: "Series.IsVerticalValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Indica se l'origine dati è verticale"
type: docs
url: /it/net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

Indica se l'origine dati è verticale.

```csharp
public bool IsVerticalValues { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsVerticalValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie con valori verticali
            chart.NSeries.Add("A1:B10", true);
            
            // Dimostra la proprietà IsVerticalValues (sola lettura)
            Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
            
            // Per cambiare l'orientamento, è necessario ricreare la serie con parametri diversi
            chart.NSeries.Clear();
            chart.NSeries.Add("A1:B10", false);
            Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


