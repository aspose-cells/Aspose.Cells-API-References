---
title: "Walls.Depth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Walls. Возвращает глубину от передней к задней стороне в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/walls/depth/
---
## Walls.Depth property

Получает глубину от передней к задней в единицах 1/4000 ширины диаграммы после вызова метода Chart.Calculate().

```csharp
public int Depth { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyDepthDemo
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

            Walls walls = chart.Walls;
            Console.WriteLine("Wall Depth: " + walls.Depth);

            workbook.Save("WallsDepthExample.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


