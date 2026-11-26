---
title: "ChartFrame.DefaultWidthRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Представляет ширину позиции по умолчанию в единицах доли области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/defaultwidthratiotochart/
---
## ChartFrame.DefaultWidthRatioToChart property

Представляет ширину позиции по умолчанию в единицах доли области диаграммы.

```csharp
public double DefaultWidthRatioToChart { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthRatioToChartDemo
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

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к заголовку диаграммы, который является ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Отобразить текущее значение DefaultWidthRatioToChart
            Console.WriteLine("Current DefaultWidthRatioToChart value: " + chartTitle.DefaultWidthRatioToChart);

            // Примечание: DefaultWidthRatioToChart только для чтения, поэтому мы не можем установить его
            // Вместо этого мы продемонстрируем его связь с фактическим коэффициентом ширины
            Console.WriteLine("Current WidthRatioToChart: " + chartTitle.WidthRatioToChart);

            // Измените коэффициент ширины, чтобы продемонстрировать его эффект
            chartTitle.WidthRatioToChart = 0.5;
            Console.WriteLine("After setting WidthRatioToChart to 0.5, DefaultWidthRatioToChart remains: " + chartTitle.DefaultWidthRatioToChart);

            // Сохраните книгу
            workbook.Save("ChartFramePropertyDefaultWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


