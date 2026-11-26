---
title: "ChartArea.HeightRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartArea. Получает или задает вертикальное смещение от строки нижнего правого угла в единицах отношения к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

Получает или задает вертикальное смещение от строки нижнего правого угла, в виде отношения к области диаграммы.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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
            chart.SetChartDataRange("A1:B4", true);

            // Получите доступ к области диаграммы
            ChartArea chartArea = chart.ChartArea;

            // Отобразить текущее значение HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Установить новое значение для HeightRatioToChart (0.5 = 50 % высоты диаграммы)
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Установить новое значение для WidthRatioToChart, чтобы продемонстрировать комбинированный эффект
            chartArea.WidthRatioToChart = 0.8;

            // Сохраните рабочую книгу, чтобы увидеть изменения
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


