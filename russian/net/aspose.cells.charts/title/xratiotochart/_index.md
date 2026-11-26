---
title: "Title.XRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Title. Возвращает или задает координату x верхнего левого угла в единицах доли области диаграммы. X в пикселях  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /ru/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

Получает или задает координату x верхнего левого угла в единицах доли области диаграммы. X в пикселях = XRatioToChart * Chart.ChartObject.Width;

```csharp
public override double XRatioToChart { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitlePropertyXRatioToChartDemo
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

            // Установить источник данных для диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить заголовок диаграммы
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // Отобразить текущее значение XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // Изменить значение XRatioToChart, чтобы переместить заголовок горизонтально
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // Сохраните книгу
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


