---
title: "AxisBins.IsAutomatic"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AxisBins. Указывает, являются ли осевые корзины автоматическими"
type: docs
url: /ru/net/aspose.cells.charts/axisbins/isautomatic/
---
## AxisBins.IsAutomatic property

Указывает, являются ли интервалы оси автоматическими.

```csharp
public bool IsAutomatic { get; set; }
```

### Примечания

Если вызывается [`Width`](../width/) или [`Count`](../count/), значение будет false.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisBinsPropertyIsAutomaticDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            Aspose.Cells.Charts.Axis valueAxis = chart.ValueAxis;
            Aspose.Cells.Charts.AxisBins bins = valueAxis.Bins;

            // Продемонстрировать свойство IsAutomatic
            bins.IsAutomatic = true;
            Console.WriteLine("Bins automatic calculation is enabled: " + bins.IsAutomatic);

            workbook.Save("AxisBinsIsAutomaticDemo.xlsx");
        }
    }
}
```

### См. также

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


