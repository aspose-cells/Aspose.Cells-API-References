---
title: "ChartFrame.DefaultHeightRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartFrame. Представляет высоту позиции по умолчанию в единицах доли области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartframe/defaultheightratiotochart/
---
## ChartFrame.DefaultHeightRatioToChart property

Представляет высоту позиции по умолчанию в единицах доли области диаграммы.

```csharp
public double DefaultHeightRatioToChart { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к заголовку диаграммы (который является ChartFrame)
            ChartFrame chartTitle = chart.Title;

            // Отобразить текущее значение DefaultHeightRatioToChart
            Console.WriteLine("Current DefaultHeightRatioToChart value: " + chartTitle.DefaultHeightRatioToChart);

            // Продемонстрировать, как это свойство влияет на диаграмму, сравнив его с HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartTitle.HeightRatioToChart);

            // Изменить коэффициент высоты, чтобы увидеть эффект
            chartTitle.HeightRatioToChart = 0.1;
            Console.WriteLine("After setting HeightRatioToChart to 0.1: " + chartTitle.HeightRatioToChart);

            // Сохраните книгу
            workbook.Save("ChartFramePropertyDefaultHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


