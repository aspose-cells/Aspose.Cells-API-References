---
title: "ChartPoint.StartAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает начальный угол для секции пирога, измеряемый в градусах по часовой стрелке от оси X после вызова метода Chart.Calculate. Применяется к круговой диаграмме."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

Получает начальный угол секции пирога, измеряемый в градусах по часовой стрелке от оси x после вызова метода Chart.Calculate(). Применяется к Pie chart.

```csharp
public float StartAngle { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
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
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы убедиться, что свойства заполнены
            chart.Calculate();

            // Получить первую точку диаграммы
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразить значение StartAngle
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // Примечание: StartAngle только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить начальный угол, нам нужно повернуть всю круговую диаграмму
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // Пересчитать, чтобы обновить углы
            chart.Calculate();

            // Отобразить новое значение StartAngle после вращения
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // Сохраните книгу
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


