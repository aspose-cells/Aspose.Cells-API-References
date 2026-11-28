---
title: "Class Marker"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.Marker sınıfı. Çizgi grafik, dağılım grafiği veya radar grafiğindeki işaretleyiciyi temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/marker/
---
## Marker class

Çizgi grafiği, dağılım grafiği veya radar grafiğindeki işareti temsil eder.

```csharp
public class Marker
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Alır [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Çizgi grafik, dağılım grafiği veya radar grafiğinde işaretleyicinin arka plan rengini temsil eder. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | İşaretleyicinin arka plan renk kümesi tipini alır veya ayarlar. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Alır [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Çizgi grafik, dağılım grafiği veya radar grafiğinde işaretleyicinin ön plan rengini temsil eder. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | İşaretçi ön plan rengi ayar türünü alır veya ayarlar. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | İşaretçi boyutunu nokta biriminde temsil eder. Çizgi grafiği, dağılım grafiği veya radar grafiği için geçerlidir. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | İşaretçi boyutunu piksel biriminde temsil eder. Çizgi grafikleri, dağılım grafikleri veya radar grafikleri için geçerlidir. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | İşaretçi stilini temsil eder. Çizgi grafiği, dağılım grafıği veya radar grafiği için geçerlidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasının referansını alın.
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleyin
            chart.NSeries.Add("A1:B3", true);

            // İlk seriye erişin
            Series series = chart.NSeries[0];

            // İşaretçi özelliklerini ayarlayın
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Çalışma kitabını kaydedin
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


