---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату Y начальной точки сектора круговой диаграммы после вызова метода Chart.Calculate. Применяется к пончиковой диаграмме."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

Получает координату y начальной точки секции пирога после вызова метода Chart.Calculate(). Применяется к Doughnut chart.

```csharp
public float InnerArcStartPointYPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // Добавить диаграмму Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы убедиться, что свойства заполнены
            chart.Calculate();

            // Получить первую точку диаграммы
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите значение InnerArcStartPointYPx
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // Примечание: InnerArcStartPointYPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить позицию, нам нужно отрегулировать размер отверстия пончика
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Пересчитайте диаграмму, чтобы обновить свойства
            chart.Calculate();

            // Отобразите новое значение InnerArcStartPointYPx после изменения размера отверстия
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // Сохраните книгу
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


