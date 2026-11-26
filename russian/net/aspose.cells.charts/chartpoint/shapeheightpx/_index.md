---
title: "ChartPoint.ShapeHeightPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Получает высоту в пикселях после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

Получает высоту в пикселях после вызова метода Chart.Calculate().

```csharp
public int ShapeHeightPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы получить размеры фигуры
            chart.Calculate();

            // Получите первую точку диаграммы из первой серии
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Отобразите текущую высоту фигуры точки диаграммы в пикселях
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // Примечание: ShapeHeightPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить высоту, нам потребуется изменить размер диаграммы или значения данных
            // и пересчитать диаграмму

            // Измените значение данных, которое повлияет на размер точки диаграммы
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // Отобразите новую высоту после изменения данных
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // Сохраните книгу
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


