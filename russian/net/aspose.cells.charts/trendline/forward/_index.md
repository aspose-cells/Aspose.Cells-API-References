---
title: "Trendline.Forward"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Возвращает или задает количество периодов или единиц на диаграмме рассеяния, на которое трендовая линия расширяется вперёд. Количество периодов должно быть больше или равно нулю."
type: docs
url: /ru/net/aspose.cells.charts/trendline/forward/
---
## Trendline.Forward property

Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое линия тренда расширяется вперёд. Количество периодов должно быть больше или равно нулю.

```csharp
public double Forward { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyForwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Добавьте линию тренда
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Продемонстрировать свойство Forward
            trendline.Forward = 2.5; // Extend trendline forward by 2.5 units
            
            workbook.Save("TrendlineForwardDemo.xlsx");
        }
    }
}
```

### См. также

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


