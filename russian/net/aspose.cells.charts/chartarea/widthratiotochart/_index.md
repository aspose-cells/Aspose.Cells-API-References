---
title: "ChartArea.WidthRatioToChart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ChartArea. Получает или задает горизонтальное смещение от столбца нижнего правого угла в единицах отношения к области диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chartarea/widthratiotochart/
---
## ChartArea.WidthRatioToChart property

Получает или задает горизонтальное смещение от столбца нижнего правого угла, в виде отношения к области диаграммы.

```csharp
public override double WidthRatioToChart { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthRatioToChartDemo
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

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Вычислить диаграмму
            chart.Calculate();

            // Продемонстрируйте свойство WidthRatioToChart
            Console.WriteLine("Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
            
            // Измените коэффициент и покажите изменение
            chart.ChartArea.WidthRatioToChart = 0.8;
            Console.WriteLine("Modified Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
        }
    }
}
```

### См. также

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


