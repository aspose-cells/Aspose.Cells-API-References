---
title: "Walls.GetCubePointXPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Walls. Возвращает координату x вершины куба стен после вызова метода Chart.Calculate. Число вершин куба стен равно восьми."
type: docs
url: /ru/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

Получает координату x вершины куба стен после вызова метода Chart.Calculate(). Количество вершин куба стен равно восьми.

```csharp
public float GetCubePointXPx(int index)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointXPxWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Создайте 3D‑диаграмму.
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Вычислите диаграмму, чтобы гарантировать доступность свойств Wall
            chart.Calculate();

            // Получить объект Walls
            Walls walls = chart.Walls;

            try
            {
                // Получите количество точек куба.
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Вызовите GetCubePointXPx с индексом 0 (первая точка).
                    float xCoordinate = walls.GetCubePointXPx(0);
                    
                    Console.WriteLine($"X coordinate of first cube point in pixels: {xCoordinate}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointXPx method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


