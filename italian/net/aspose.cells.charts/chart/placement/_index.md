---
title: "Chart.Placement"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Rappresenta il modo in cui il grafico è collegato alle celle sottostanti"
type: docs
url: /it/net/aspose.cells.charts/chart/placement/
---
## Chart.Placement property

Rappresenta il modo in cui il grafico è collegato alle celle sottostanti.

```csharp
public PlacementType Placement { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlacementDemo
    {
        public static void Run()
        {
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

            // Aggiungi un grafico e imposta i dati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Dimostra la proprietà Placement
            chart.Placement = PlacementType.MoveAndSize;
            Console.WriteLine("Chart Placement: " + chart.Placement);

            workbook.Save("ChartPlacementDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


