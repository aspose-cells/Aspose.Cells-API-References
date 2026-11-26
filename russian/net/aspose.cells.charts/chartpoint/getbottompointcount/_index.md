---
title: "ChartPoint.GetBottomPointCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartPoint. Получает количество нижних точек после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/getbottompointcount/
---
## ChartPoint.GetBottomPointCount method

Получает количество нижних точек после вызова метода Chart.Calculate().

```csharp
public int GetBottomPointCount()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointCountDemo
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
            
            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Вычислите диаграмму, чтобы убедиться, что все точки рассчитаны
            chart.Calculate();
            
            try
            {
                // Получите первую точку в первой серии.
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Вызовите метод GetBottomPointCount
                int bottomPointCount = point.GetBottomPointCount();
                
                // Отобразить результат
                Console.WriteLine($"Number of bottom points: {bottomPointCount}");
                
                // Покажите координаты нижних точек
                for (int i = 0; i < bottomPointCount; i++)
                {
                    float x = point.GetBottomPointXPx(i);
                    float y = point.GetBottomPointYPx(i);
                    Console.WriteLine($"Bottom point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointCount method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodGetBottomPointCountDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


