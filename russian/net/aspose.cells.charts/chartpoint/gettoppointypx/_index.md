---
title: "ChartPoint.GetTopPointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartPoint. Получает y‑координату верхней точки фигуры после вызова метода Chart.Calculate. Применяется к 3D‑диаграммам Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/gettoppointypx/
---
## ChartPoint.GetTopPointYPx method

Получает координату y верхней точки формы после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid и Area3D.

```csharp
public float GetTopPointYPx(int index)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointYPxWithInt32Demo
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
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Выполните расчёт диаграммы, чтобы убедиться, что все свойства позиции вычислены
            chart.Calculate();
            
            // Получите первую точку диаграммы из первой серии
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Получите количество верхних точек
                int topPointCount = point.GetTopPointCount();
                
                if (topPointCount > 0)
                {
                    // Вызовите GetTopPointYPx с индексом 0
                    float yPx = point.GetTopPointYPx(0);
                    
                    Console.WriteLine($"Top point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointYPx method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ChartPointMethodGetTopPointYPxWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


