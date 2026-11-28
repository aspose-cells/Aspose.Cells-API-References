---
title: "Marker.MarkerSizePx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Marker özelliği. İşaretleyicinin boyutunu piksel biriminde temsil eder. Çizgi grafikleri, dağılım grafikleri veya radar grafiklerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/marker/markersizepx/
---
## Marker.MarkerSizePx property

İşaretçi boyutunu piksel biriminde temsil eder. Çizgi grafikleri, dağılım grafikleri veya radar grafikleri için geçerlidir.

```csharp
public int MarkerSizePx { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


