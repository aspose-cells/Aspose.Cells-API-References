---
title: "Marker.MarkerSizePx"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Marker. تمثل حجم العلامة بوحدات البكسل. ينطبق على المخططات الخطية والمخططات المبعثرة أو مخططات الرادار"
type: docs
url: /ar/net/aspose.cells.charts/marker/markersizepx/
---
## Marker.MarkerSizePx property

يمثل حجم العلامة بوحدات البكسل. ينطبق على مخططات الخط، المخططات المبعثرة، أو مخططات الرادار.

```csharp
public int MarkerSizePx { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizePxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            chart.NSeries.Add("A1:B3", true);
            Series series = chart.NSeries[0];

            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSizePx = 20;
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            workbook.Save("MarkerSizePxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


