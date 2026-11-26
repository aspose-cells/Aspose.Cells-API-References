---
title: "Title.YRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Title. Возвращает или задает координату y верхнего левого угла в единицах доли области диаграммы. Y в пикселях  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /ru/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

Получает или задает координату y верхнего левого угла в единицах доли области диаграммы. Y в пикселях = YRatioToChart * Chart.ChartObject.Width;

```csharp
public override double YRatioToChart { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyYRatioToChartDemo
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

            // Получить заголовок диаграммы
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // Отобразить текущее значение YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // Изменить свойство YRatioToChart, чтобы переместить заголовок вертикально
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // Сохраните книгу
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


