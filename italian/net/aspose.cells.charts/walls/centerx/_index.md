---
title: "Walls.CenterX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Walls. Restituisce la coordinata x dell'angolo sinistro inferiore del centro del muro in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/walls/centerx/
---
## Walls.CenterX property

Ottiene la coordinata x dell'angolo sinistro-inferiore del centro della parete in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate().

```csharp
public int CenterX { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            Walls walls = chart.Walls;
            Console.WriteLine("Wall CenterX position: " + walls.CenterX);

            workbook.Save("WallsCenterXExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


