---
title: "ChartPoint.GetOnCategoryAxisPointXPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ChartPoint method. Получает координату x точки на категориальной оси после вызова метода Chart.Calculate. Применяется только к диаграмме Area."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/getoncategoryaxispointxpx/
---
## ChartPoint.GetOnCategoryAxisPointXPx method

Получает координату x точки на оси категорий после вызова метода Chart.Calculate(). Применяется только к Area chart.

```csharp
public float GetOnCategoryAxisPointXPx(int index)
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

    public class ChartPointMethodGetOnCategoryAxisPointXPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислить диаграмму
            chart.Calculate();

            try
            {
                // Получить первую точку диаграммы
                ChartPoint point = chart.NSeries[0].Points[0];

                // Вызвать GetOnCategoryAxisPointXPx с индексом 0
                float xPosition = point.GetOnCategoryAxisPointXPx(0);

                // Отобразить результат
                Console.WriteLine($"X position of first category axis point: {xPosition} pixels");

                // Сохраните книгу
                workbook.Save("ChartPointGetOnCategoryAxisPointXPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointXPx method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


