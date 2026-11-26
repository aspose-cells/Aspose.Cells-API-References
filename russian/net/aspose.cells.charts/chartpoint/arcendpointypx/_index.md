---
title: "ChartPoint.ArcEndPointYPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает координату y конечной точки сектора круговой диаграммы после вызова метода Chart.Calculate. Применяется к диаграммам Pie и Doughnut."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/arcendpointypx/
---
## ChartPoint.ArcEndPointYPx property

Получает координату y конечной точки секции круговой диаграммы после вызова метода Chart.Calculate(). Применяется к круговым и кольцевым диаграммам.

```csharp
public float ArcEndPointYPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(12000);
            worksheet.Cells["B4"].PutValue(14000);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы получить позиции фигур.
            chart.Calculate();

            // Получить первую точку диаграммы
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите текущее значение ArcEndPointYPx.
            Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);

            // Поскольку ArcEndPointYPx только для чтения, мы можем лишь прочитать его.
            // Следующая строка вызовет ошибку компиляции:
            // point.ArcEndPointYPx = 150.5f;

            // Продемонстрируйте, как это свойство влияет на круговую диаграмму.
            Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");

            // Сохраните книгу
            workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


