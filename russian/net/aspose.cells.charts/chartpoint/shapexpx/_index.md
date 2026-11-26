---
title: "ChartPoint.ShapeXPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату X верхнего левого угла в пикселях после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/shapexpx/
---
## ChartPoint.ShapeXPx property

Получает координату x верхнего левого угла в пикселях после вызова метода Chart.Calculate().

```csharp
public int ShapeXPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXPxDemo
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

            // Получите первую точку диаграммы из первой серии
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить текущую позицию X в пикселях
            Console.WriteLine("Current ShapeXPx value: " + point.ShapeXPx);

            // Примечание: ShapeXPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить позицию, нам потребуется изменить размер/позицию диаграммы или данные

            // Продемонстрировать, как свойство меняется при изменении диаграммы
            Console.WriteLine("\nChanging chart position...");
            chart.ChartObject.Left = 3;
            chart.ChartObject.Top = 2;
            chart.Calculate(); // Recalculate to update positions

            Console.WriteLine("New ShapeXPx value after chart move: " + point.ShapeXPx);

            // Сохранить результат
            workbook.Save("ChartPointPropertyShapeXPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


