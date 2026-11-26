---
title: "Walls.CenterXPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Walls. Получает x‑координату левого нижнего угла центра Wall в пикселях после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/walls/centerxpx/
---
## Walls.CenterXPx property

Получает координату x нижнего левого угла центра стены в пикселях после вызова метода Chart.Calculate().

```csharp
public int CenterXPx { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterXPxDemo
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
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);

            workbook.Save("WallsCenterXPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


