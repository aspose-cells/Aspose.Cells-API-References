---
title: "Trendline.Period"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Возвращает или задает период для трендовой линии скользящего среднего"
type: docs
url: /ru/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

Возвращает или задает период для линии тренда скользящего среднего.

```csharp
public int Period { get; set; }
```

### Примечания

Это значение должно быть в диапазоне от 2 до 255. И оно должно быть меньше количества точек диаграммы в серии.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Добавьте трендовую линию скользящего среднего
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // Сохраните книгу
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### См. также

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


