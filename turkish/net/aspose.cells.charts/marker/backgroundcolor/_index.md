---
title: "Marker.BackgroundColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Marker özelliği. Çizgi grafiği, dağılım grafiği veya radar grafiğinde işaretleyicinin arka plan rengini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Çizgi grafik, dağılım grafiği veya radar grafiğinde işaretleyicinin arka plan rengini temsil eder.

```csharp
public Color BackgroundColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // İşaretleyici görünümünü özelleştir
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.Circle;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = System.Drawing.Color.Blue;
                series.Marker.BackgroundColor = System.Drawing.Color.LightGreen; // Demonstrating BackgroundColor property
            }

            workbook.Save("MarkerBackgroundColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


