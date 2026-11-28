---
title: "Marker.ForegroundColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Marker özelliği. Çizgi grafiği, dağılım grafiği veya radar grafiğinde işaretleyicinin ön plan rengini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/marker/foregroundcolor/
---
## Marker.ForegroundColor property

Çizgi grafik, dağılım grafiği veya radar grafiğinde işaretleyicinin ön plan rengini temsil eder.

```csharp
public Color ForegroundColor { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyForegroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            Marker marker = chart.NSeries[0].Marker;
            marker.MarkerStyle = ChartMarkerType.Circle;
            marker.MarkerSize = 10;
            marker.ForegroundColor = Color.Red;

            workbook.Save("MarkerForegroundColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


