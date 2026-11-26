---
title: "Walls.WidthPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Walls. Получает ширину слева направо в пикселях после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/walls/widthpx/
---
## Walls.WidthPx property

Получает ширину слева направо в пикселях после вызова метода Chart.Calculate().

```csharp
public int WidthPx { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyWidthPxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить 3D‑диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Получить walls и продемонстрировать свойство WidthPx
            Walls walls = chart.Walls;
            Console.WriteLine("Wall width in pixels: " + walls.WidthPx);

            // Сохранить книгу
            workbook.Save("WallsWidthPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


