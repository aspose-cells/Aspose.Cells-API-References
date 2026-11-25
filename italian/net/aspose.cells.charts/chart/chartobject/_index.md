---
title: "Chart.ChartObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Rappresenta il chartShape"
type: docs
url: /it/net/aspose.cells.charts/chart/chartobject/
---
## Chart.ChartObject property

Rappresenta il chartShape;

```csharp
public ChartShape ChartObject { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartObjectDemo
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

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra le proprietà di ChartObject
            chart.ChartObject.Placement = PlacementType.Move;
            chart.ChartObject.X = 100;
            chart.ChartObject.Y = 200;
            chart.ChartObject.Width = 400;
            chart.ChartObject.Height = 300;

            // Salva la cartella di lavoro
            workbook.Save("ChartObjectDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ChartShape](../../../aspose.cells.drawing/chartshape/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


