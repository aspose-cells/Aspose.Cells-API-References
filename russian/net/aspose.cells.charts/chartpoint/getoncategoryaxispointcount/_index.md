---
title: "ChartPoint.GetOnCategoryAxisPointCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartPoint. Возвращает количество точек на категориальной оси после вызова метода Chart.Calculate. Применяется только к областным диаграммам."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/getoncategoryaxispointcount/
---
## ChartPoint.GetOnCategoryAxisPointCount method

Получает количество точек на оси категорий после вызова метода Chart.Calculate(). Применяется только к area charts.

```csharp
public int GetOnCategoryAxisPointCount()
```

### Примечания

Для 2D-областной диаграммы возвращается 1, для 3D‑областной диаграммы — 2.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointCountDemo
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

            // Добавьте областную диаграмму.
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Выполните расчёт диаграммы, чтобы убедиться, что все точки диаграммы вычислены.
            chart.Calculate();

            try
            {
                // Получите первую точку диаграммы из первой серии
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Вызовите метод GetOnCategoryAxisPointCount.
                int pointCount = point.GetOnCategoryAxisPointCount();
                
                Console.WriteLine($"Number of points on category axis: {pointCount}");
                
                // Отобразите координаты каждой точки на категориальной оси.
                for (int i = 0; i < pointCount; i++)
                {
                    float x = point.GetOnCategoryAxisPointXPx(i);
                    float y = point.GetOnCategoryAxisPointYPx(i);
                    Console.WriteLine($"Point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointCount method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("MethodGetOnCategoryAxisPointCountDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


