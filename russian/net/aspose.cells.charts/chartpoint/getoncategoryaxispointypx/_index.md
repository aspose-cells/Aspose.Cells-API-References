---
title: "ChartPoint.GetOnCategoryAxisPointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ChartPoint. Возвращает координату y точки на оси категорий после вызова метода Chart.Calculate. Применяется только к диаграмме Area"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/getoncategoryaxispointypx/
---
## ChartPoint.GetOnCategoryAxisPointYPx method

Получает координату y точки на оси категорий после вызова метода Chart.Calculate(). Применяется только к диаграмме Area.

```csharp
public float GetOnCategoryAxisPointYPx(int index)
```

### Примечания

Диаграмма Area 2D: индекс 0. Диаграмма Area 3D: индекс 0 или 1.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
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
                // Вызовите GetOnCategoryAxisPointYPx с индексом 0
                float yPx = point.GetOnCategoryAxisPointYPx(0);
                
                // Отобразить результат
                Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
                
                // Сохраните книгу
                workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


