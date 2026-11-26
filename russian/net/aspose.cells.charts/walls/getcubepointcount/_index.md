---
title: "Walls.GetCubePointCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Walls. Получает количество точек куба после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

Получает количество точек куба после вызова метода Chart.Calculate().

```csharp
public int GetCubePointCount()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Добавить 3D‑диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы гарантировать доступность свойств Wall
            chart.Calculate();

            try
            {
                // Получить объект Walls
                Walls walls = chart.Walls;
                
                // Вызвать метод GetCubePointCount
                int pointCount = walls.GetCubePointCount();
                
                // Отобразить результат
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // Сохраните книгу
                workbook.Save("WallsMethodGetCubePointCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointCount method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


