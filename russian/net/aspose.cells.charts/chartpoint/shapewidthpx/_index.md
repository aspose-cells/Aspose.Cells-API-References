---
title: "ChartPoint.ShapeWidthPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает ширину в пикселях после вызова метода Chart.Calculate"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

Получает ширину в пикселях после вызова метода Chart.Calculate().

```csharp
public int ShapeWidthPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы обеспечить доступность свойств фигур.
            chart.Calculate();

            // Получите первую точку диаграммы из первой серии
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить текущую ширину формы точки диаграммы в пикселях
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // Примечание: ShapeWidthPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить ширину, нам нужно изменить размер диаграммы или другие свойства
            // это повлияет на ширину точки при следующем вызове Calculate()

            // Измените ширину диаграммы, чтобы продемонстрировать, как это влияет на ShapeWidthPx
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // Отобразить новую ширину после изменения размера диаграммы
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // Сохранить результат
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


