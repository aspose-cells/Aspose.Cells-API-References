---
title: "ChartPoint.ArcStartPointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату y начальной точки секции pie после вызова метода Chart.Calculate. Применяется к диаграммам Pie и Doughnut."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

Получает координату y начальной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к круговым и кольцевым диаграммам.

```csharp
public float ArcStartPointYPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
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

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы получить позиции фигур.
            chart.Calculate();

            // Получить первую точку диаграммы
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить текущее значение ArcStartPointYPx.
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // Примечание: ArcStartPointYPx только для чтения, поэтому мы не можем установить его напрямую
            // Вместо этого мы продемонстрируем, как изменение других свойств влияет на ArcStartPointYPx

            // Измените значение взрыва, чтобы изменить положение сектора круговой диаграммы
            point.Explosion = 20;

            // Пересчитайте диаграмму, чтобы обновить позиции
            chart.Calculate();

            // Отобразите новое значение ArcStartPointYPx после изменения взрыва
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // Сохраните книгу
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


