---
title: "ChartPoint.RadiusPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartPoint. Возвращает радиус пузырьковой, круговой или пончиковой диаграммы в пикселях после вызова метода Chart.Calculate."
type: docs
url: /ru/net/aspose.cells.charts/chartpoint/radiuspx/
---
## ChartPoint.RadiusPx property

Получает радиус пузыря, сектора или кольца в пикселях после вызова метода Chart.Calculate().

```csharp
public int RadiusPx { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyRadiusPxDemo
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
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислите диаграмму, чтобы убедиться, что свойства заполнены
            chart.Calculate();

            // Получить первую точку диаграммы
            ChartPoint point = chart.NSeries[0].Points[0];

            // Отобразите текущее значение радиуса
            Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);

            // Примечание: RadiusPx только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы изменить радиус, нам нужно отрегулировать размер диаграммы или другие свойства
            // которые влияют на размер точки косвенно

            // Пример того, как изменение размера диаграммы влияет на радиус
            Console.WriteLine("\nChanging chart size to demonstrate radius change...");
            chart.ChartObject.Width = 800;
            chart.ChartObject.Height = 600;
            chart.Calculate();

            // Отобразите новое значение радиуса после изменения размера диаграммы
            Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);

            // Сохранить результат
            workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


