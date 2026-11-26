---
title: "ChartPoint.EndAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает конечный угол секции pie, измеряемый в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate. Применяется к диаграмме Pie."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

Получает конечный угол секции круговой диаграммы, измеряемый в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate(). Применяется к круговой диаграмме.

```csharp
public float EndAngle { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы pie.
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы убедиться, что свойства заполнены
            chart.Calculate();

            // Получите первую точку диаграммы (сектор Apple).
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить текущее значение EndAngle.
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // Примечание: EndAngle только для чтения, поэтому мы не можем установить его напрямую.
            // Вместо этого мы покажем, как он соотносится с сектором pie.

            // Взрывьте точку, чтобы увидеть, как это влияет на углы.
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // Отобразить новое значение EndAngle после взрыва.
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // Сохраните книгу
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


