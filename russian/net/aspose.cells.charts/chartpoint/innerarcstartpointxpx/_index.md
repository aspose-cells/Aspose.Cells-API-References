---
title: "ChartPoint.InnerArcStartPointXPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату x начальной точки секции пирога после вызова метода Chart.Calculate. Применяется к диаграмме Doughnut"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/innerarcstartpointxpx/
---
## ChartPoint.InnerArcStartPointXPx property

Получает координату x начальной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к кольцевой диаграмме.

```csharp
public float InnerArcStartPointXPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму Doughnut
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Выполните расчёт диаграммы, чтобы получить свойства формы
            chart.Calculate();

            // Получить первую точку диаграммы
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить значение InnerArcStartPointXPx
            Console.WriteLine("InnerArcStartPointXPx: " + point.InnerArcStartPointXPx);

            // Примечание: InnerArcStartPointXPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить позицию, нам потребуется изменить размер диаграммы или размер отверстия Doughnut

            // Сохраните книгу
            workbook.Save("ChartPointPropertyInnerArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


