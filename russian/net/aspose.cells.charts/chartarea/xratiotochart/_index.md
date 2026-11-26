---
title: "ChartArea.XRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartArea. Получает или задает горизонтальное смещение от столбца верхнего левого угла как отношение к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

Получает или задает горизонтальное смещение от столбца верхнего‑левого угла, как отношение к области диаграммы.

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

    public class ChartAreaPropertyXRatioToChartDemo
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

            // Получите область диаграммы
            ChartArea chartArea = chart.ChartArea;

            // Отобразите текущее значение XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // Измените значение XRatioToChart, чтобы переместить область диаграммы горизонтально
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // Отобразите новое значение XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // Сохраните книгу
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### См. также

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


