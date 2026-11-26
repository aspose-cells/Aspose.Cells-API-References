---
title: "Series.TrendLines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает все линии тренда этой серии"
type: docs
url: /ru/net/aspose.cells.charts/series/trendlines/
---
## Series.TrendLines property

Возвращает все линии тренда этого ряда.

```csharp
public TrendlineCollection TrendLines { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyTrendLinesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Добавьте диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Добавьте экспоненциальную линию тренда к первой серии и получите её по индексу
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;

            // Сохраните книгу
            workbook.Save("TrendLinesDemo.xlsx");
        }
    }
}
```

### См. также

* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


