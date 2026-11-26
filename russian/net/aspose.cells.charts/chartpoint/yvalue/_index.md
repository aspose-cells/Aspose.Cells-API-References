---
title: "ChartPoint.YValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает или задает значение Y точки диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/yvalue/
---
## ChartPoint.YValue property

Получает или задает значение Y chartpoint.

```csharp
public object YValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyYValueDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Получить точки первой серии
            Series series = chart.NSeries[0];
            var points = series.Points;

            // Продемонстрировать свойство YValue
            Console.WriteLine("Y Values of Chart Points:");
            for (int i = 0; i < points.Count; i++)
            {
                Console.WriteLine($"Point {i + 1}: {points[i].YValue}");
            }

            // Изменить YValue точки
            points[2].YValue = 50;
            Console.WriteLine($"\nModified Point 3 YValue to: {points[2].YValue}");

            // Сохраните книгу
            workbook.Save("ChartPointYValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


