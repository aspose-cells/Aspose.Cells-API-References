---
title: "Walls.HeightPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Walls. Ottiene l'altezza dall'alto verso il basso in unità di pixel dopo la chiamata al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/walls/heightpx/
---
## Walls.HeightPx property

Ottiene l'altezza dall'alto verso il basso in unità di pixel dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int HeightPx { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyHeightPxDemo
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

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            Walls walls = chart.Walls;
            Console.WriteLine("Wall height in pixels: " + walls.HeightPx);

            workbook.Save("WallsHeightPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


