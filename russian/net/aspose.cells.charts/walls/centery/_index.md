---
title: "Walls.CenterY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Walls. Возвращает координату y левого нижнего угла центра стены в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/walls/centery/
---
## Walls.CenterY property

Получает координату y левого нижнего угла центра стены в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate().

```csharp
public int CenterY { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WallsPropertyCenterYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить 3D‑диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column3D, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы обновить свойства.
            chart.Calculate();

            // Получите доступ к walls и продемонстрируйте свойство CenterY.
            Aspose.Cells.Charts.Walls walls = chart.Walls;
            Console.WriteLine("Wall CenterY position: " + walls.CenterY);

            // Сохраните книгу
            workbook.Save("WallsCenterYDemo.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


