---
title: "Walls.GetCubePointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Walls. Получает y‑координату вершины куба стен после вызова метода Chart.Calculate. Количество вершин куба стен равно восьми"
type: docs
url: /ru/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

Получает координату y вершины куба стен после вызова метода Chart.Calculate(). Количество вершин куба стен равно восьми.

```csharp
public float GetCubePointYPx(int index)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointYPxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить 3D‑диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы гарантировать заполнение свойств Wall
            chart.Calculate();

            // Получить объект Walls
            Walls walls = chart.Walls;

            try
            {
                // Получить количество точек куба
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Вызвать GetCubePointYPx с первым индексом (0)
                    float yPx = walls.GetCubePointYPx(0);
                    Console.WriteLine($"Y-coordinate of first cube point in pixels: {yPx}");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointYPx method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


