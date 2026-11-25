---
title: "ChartCalculateOptions.ChartCalculateOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore ChartCalculateOptions. Crea le opzioni per il calcolo del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartcalculateoptions/chartcalculateoptions/
---
## ChartCalculateOptions constructor

Crea le opzioni per il calcolo del grafico.

```csharp
public ChartCalculateOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsMethodCtorDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Crea ChartCalculateOptions usando il costruttore
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;
            
            // Ricalcola il grafico con le opzioni
            chart.Calculate(calculateOptions);

            // Salva la cartella di lavoro
            workbook.Save("ChartCalculateOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


