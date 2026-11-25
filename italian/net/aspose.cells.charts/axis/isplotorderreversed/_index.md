---
title: "Axis.IsPlotOrderReversed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Indica se Microsoft Excel traccia i punti dati dall'ultimo al primo"
type: docs
url: /it/net/aspose.cells.charts/axis/isplotorderreversed/
---
## Axis.IsPlotOrderReversed property

Rappresenta se Microsoft Excel traccia i punti dati dall'ultimo al primo.

```csharp
public bool IsPlotOrderReversed { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsPlotOrderReversedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Inverti l'ordine di visualizzazione delle categorie
            chart.CategoryAxis.IsPlotOrderReversed = true;

            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyIsPlotOrderReversedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


