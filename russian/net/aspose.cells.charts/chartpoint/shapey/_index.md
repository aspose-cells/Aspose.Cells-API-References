---
title: "ChartPoint.ShapeY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату y верхнего левого угла в единицах 1/4000 высоты диаграммы после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/shapey/
---
## ChartPoint.ShapeY property

Получает координату y верхнего левого угла в единицах 1/4000 от высоты диаграммы после вызова метода Chart.Calculate().

```csharp
public int ShapeY { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYDemo
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

            // Вычислите диаграмму, чтобы получить позиции фигур
            chart.Calculate();

            // Получите первую точку в первой серии.
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите текущее значение ShapeY (1/4000 высоты диаграммы).
            Console.WriteLine("Current ShapeY value: " + point.ShapeY);

            // Примечание: ShapeY доступен только для чтения, поэтому мы не можем установить его напрямую.
            // Чтобы изменить позицию, нам потребуется изменить исходные данные или свойства диаграммы.

            // Продемонстрируйте, как ShapeY соотносится с фактической позицией.
            Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
            Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));

            // Сохранить результат
            workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


