---
title: "ChartPoint.InnerRadiusPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает внутренний радиус сектора кольцевой диаграммы в пикселях после вызова метода Chart.Calculate. Применяется к диаграмме Doughnut."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

Возвращает внутренний радиус сектора кольцевой диаграммы в пикселях после вызова метода Chart.Calculate(). Применяется к диаграмме Doughnut.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство устарело. Вместо него используйте свойство ChartPoint.DoughnutInnerRadius. Это свойство будет удалено через 12 месяцев, начиная с июня 2024 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
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
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Добавить диаграмму Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы получить свойства точек диаграммы.
            chart.Calculate();

            // Получите первую точку диаграммы из первой серии
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите текущее значение внутреннего радиуса (свойство только для чтения).
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // Примечание: InnerRadiusPx только для чтения, поэтому установить его напрямую нельзя.
            // Чтобы изменить внутренний радиус, необходимо скорректировать размер отверстия кольца.
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Пересчитайте диаграмму, чтобы обновить свойства
            chart.Calculate();

            // Отобразите новое значение внутреннего радиуса после изменения размера отверстия кольца.
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // Сохранить результат
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


