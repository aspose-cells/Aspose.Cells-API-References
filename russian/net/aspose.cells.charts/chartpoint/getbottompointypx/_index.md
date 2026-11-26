---
title: "ChartPoint.GetBottomPointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ChartPoint method. Получает координату y нижней точки фигуры после вызова метода Chart.Calculate. Применяется к 3D‑диаграммам Column3D, Bar3D, Cone, Cylinder, Pyramid."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/getbottompointypx/
---
## ChartPoint.GetBottomPointYPx method

Получает координату y нижней точки формы после вызова метода Chart.Calculate(). Применяется к 3D‑диаграммам: Column3D, Bar3D, Cone, Cylinder, Pyramid.

```csharp
public float GetBottomPointYPx(int index)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointYPxDemo
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
            
            // Добавить серию
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Вычислите диаграмму, чтобы убедиться, что все точки рассчитаны
            chart.Calculate();
            
            // Получить первую точку первой серии
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Получить количество нижних точек
                int bottomPointCount = point.GetBottomPointCount();
                
                if (bottomPointCount > 0)
                {
                    // Вызвать GetBottomPointYPx с индексом 0
                    float yPx = point.GetBottomPointYPx(0);
                    
                    Console.WriteLine($"Bottom point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointYPx method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("MethodGetBottomPointYPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


