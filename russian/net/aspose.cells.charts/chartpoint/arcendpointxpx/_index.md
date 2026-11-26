---
title: "ChartPoint.ArcEndPointXPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату x конечной точки секции пирога после вызова метода Chart.Calculate. Применяется к диаграммам Pie и Doughnut"
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/arcendpointxpx/
---
## ChartPoint.ArcEndPointXPx property

Получает координату x конечной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к круговым и кольцевым диаграммам.

```csharp
public float ArcEndPointXPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointXPxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы убедиться, что свойства заполнены
            chart.Calculate();

            // Получить первую точку диаграммы
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить значение ArcEndPointXPx
            Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);

            // Примечание: ArcEndPointXPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить конечную точку, нам нужно изменить данные диаграммы или свойства, влияющие на кусок пирога
            
            // Пример того, как изменение данных влияет на ArcEndPointXPx
            worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
            chart.Calculate(); // Recalculate chart

            // Отобразить новое значение ArcEndPointXPx после изменения данных
            Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);

            // Сохраните книгу
            workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


