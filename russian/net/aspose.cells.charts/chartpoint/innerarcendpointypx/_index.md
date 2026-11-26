---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату Y конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate. Применяется к пончиковой диаграмме."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

Получает координату y конечной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к кольцевой диаграмме.

```csharp
public float InnerArcEndPointYPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // Добавить диаграмму Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Выполните расчёт диаграммы, чтобы получить свойства точек диаграммы
            chart.Calculate();

            // Получите первую точку диаграммы из первой серии
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите текущее значение InnerArcEndPointYPx
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // Примечание: InnerArcEndPointYPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить позицию, нам нужно изменить размер отверстия пончика
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // Пересчитайте диаграмму, чтобы обновить свойства
            chart.Calculate();

            // Отобразите новое значение InnerArcEndPointYPx после изменения размера отверстия
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // Сохраните книгу
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


