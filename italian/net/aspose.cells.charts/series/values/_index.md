---
title: "Series.Values"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Rappresenta i valori Y di questa serie di grafico"
type: docs
url: /it/net/aspose.cells.charts/series/values/
---
## Series.Values property

Rappresenta i valori Y di questa serie di grafico.

```csharp
public string Values { get; set; }
```

### Osservazioni

Per ottenere i valori effettivi (corrispondenti a ogni punto di questa serie) definiti da questa proprietà, si prega di utilizzare [`PointValues`](../pointvalues/).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi una serie usando la proprietà Values
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.Add("=Sheet1!$C$2:$C$4", true);

            // Imposta i dati di categoria
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Visualizza la proprietà Values per ogni serie
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            Console.WriteLine("Series 2 Values: " + chart.NSeries[1].Values);

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyValuesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


