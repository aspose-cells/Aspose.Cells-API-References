---
title: "ChartPoint.Marker"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. İşaretçiyi alır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/marker/
---
## ChartPoint.Marker property

` marker`'ı alır.

```csharp
public Marker Marker { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(150);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(33);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Scatter, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            
            // İlk nokta için işaretçiyi özelleştirin.
            int pointIndex = 0;
            chart.NSeries[0].Points[pointIndex].Marker.Border.Color = Color.Yellow;
            chart.NSeries[0].Points[pointIndex].Marker.Area.ForegroundColor = Color.Green;
            chart.NSeries[0].Points[pointIndex].Marker.MarkerStyle = Aspose.Cells.Charts.ChartMarkerType.Circle;
            chart.NSeries[0].Points[pointIndex].Marker.MarkerSize = 16;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointMarkerDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Marker](../../marker/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


