---
title: "Line.BeginArrowWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает ширину наконечника стрелки для начала линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/beginarrowwidth/
---
## Line.BeginArrowWidth property

Указывает ширину наконечника стрелки для начала линии.

```csharp
public MsoArrowheadWidth BeginArrowWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginArrowWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Добавьте трендлайн и задайте свойства стрелки
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.BeginType = MsoArrowheadStyle.Arrow;
            trendline.BeginArrowWidth = MsoArrowheadWidth.Wide;
            trendline.EndType = MsoArrowheadStyle.Arrow;
            trendline.EndArrowWidth = MsoArrowheadWidth.Narrow;

            workbook.Save("LinePropertyBeginArrowWidthDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


