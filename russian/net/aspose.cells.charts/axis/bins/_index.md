---
title: "Axis.Bins"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет интервалы на оси гистограммы/парето"
type: docs
url: /ru/net/aspose.cells.charts/axis/bins/
---
## Axis.Bins property

Представляет интервалы на оси диаграммы (гистограмма/Pareto)

```csharp
public AxisBins Bins { get; }
```

### Примечания

Только для гистограммы или диаграммы Парето.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBinsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Создать гистограмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Настроить интервалы
            AxisBins bins = chart.ValueAxis.Bins;
            bins.IsAutomatic = false;
            bins.Width = 15;
            bins.Overflow = 55;
            bins.Underflow = 5;

            workbook.Save("AxisBinsDemo.xlsx");
        }
    }
}
```

### См. также

* class [AxisBins](../../axisbins/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


