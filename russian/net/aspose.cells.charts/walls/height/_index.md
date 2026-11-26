---
title: "Walls.Height"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Walls. Возвращает высоту от верхней до нижней части в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/walls/height/
---
## Walls.Height property

Получает высоту сверху вниз в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate().

```csharp
public int Height { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyHeightDemo
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

            // Получите доступ к walls и продемонстрируйте свойство Height.
            Walls walls = chart.Walls;
            Console.WriteLine("Wall Height: " + walls.Height);
            Console.WriteLine("Wall Height in Pixels: " + walls.HeightPx);

            // Измените размер области диаграммы вместо прямого использования свойства Height.
            chart.ChartObject.Height = 400;
            chart.Calculate();
            Console.WriteLine("After resizing - Wall Height: " + walls.Height);
            Console.WriteLine("After resizing - Wall Height in Pixels: " + walls.HeightPx);

            workbook.Save("WallsHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


