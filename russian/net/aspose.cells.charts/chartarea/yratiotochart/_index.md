---
title: "ChartArea.YRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartArea. Получает или получает вертикальное смещение от строки верхнего левого угла в единицах отношения к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

Получает или получает вертикальное смещение от строки верхнего левого угла, в виде отношения к области диаграммы.

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

    public class ChartAreaPropertyYRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получите доступ к области диаграммы
            ChartArea chartArea = chart.ChartArea;

            // Отобразить текущее значение YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // Изменить свойство YRatioToChart (0.0–1.0 представляет 0 %–100 % области диаграммы)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // Отобразить новое значение YRatioToChart
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


