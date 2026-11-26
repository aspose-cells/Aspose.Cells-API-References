---
title: "ChartPoint.GetTopPointXPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartPoint. Возвращает x‑координату верхней точки формы после вызова метода Chart.Calculate. Применяется к 3D‑диаграммам Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/gettoppointxpx/
---
## ChartPoint.GetTopPointXPx method

Получает координату x верхней точки формы после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D.

```csharp
public float GetTopPointXPx(int index)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointXPxWithInt32Demo
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

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Выполните расчёт диаграммы, чтобы убедиться, что все свойства позиции вычислены
            chart.Calculate();

            try
            {
                // Получите первую точку диаграммы из первой серии
                ChartPoint point = chart.NSeries[0].Points[0];

                // Получите количество верхних точек
                int pointCount = point.GetTopPointCount();

                if (pointCount > 0)
                {
                    // Вызвать GetTopPointXPx с индексом 0
                    float xPos = point.GetTopPointXPx(0);
                    Console.WriteLine($"X position of top point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }

                Console.WriteLine("Method executed successfully with parameters (Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointXPx method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("ChartPointMethodGetTopPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


