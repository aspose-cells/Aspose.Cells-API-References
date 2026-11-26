---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Справочник API Aspose.Cells для .NET"
description: "ChartPoint property. Получает внутренний радиус сектора кольцевой диаграммы в пикселях после вызова метода Chart.Calculate. Применяется к кольцевой диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

Получает внутренний радиус сектора кольцевой диаграммы в пикселях после вызова метода Chart.Calculate(). Применяется к кольцевой диаграмме.

```csharp
public int DoughnutInnerRadius { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
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
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы получить точки диаграммы
            chart.Calculate();

            // Получите первую точку диаграммы из первой серии
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите текущее значение DoughnutInnerRadius
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Примечание: DoughnutInnerRadius только для чтения, поэтому его нельзя установить напрямую
            // Чтобы изменить внутренний радиус, необходимо отрегулировать свойство HoleSize диаграммы
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // Пересчитайте диаграмму, чтобы обновить DoughnutInnerRadius
            chart.Calculate();

            // Отобразите обновлённое значение DoughnutInnerRadius
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Сохраните книгу
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


