---
title: "Marker.MarkerSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Marker özelliği. İşaretçi boyutunu puan biriminde temsil eder. Çizgi grafiği, dağılım grafiği veya radar grafiği için geçerlidir."
type: docs
url: /tr/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

İşaretçi boyutunu nokta biriminde temsil eder. Çizgi grafiği, dağılım grafiği veya radar grafiği için geçerlidir.

```csharp
public int MarkerSize { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Seri ekle - düzeltilmiş yöntem çağrısı
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // İşaretçi özelliklerini ayarlayın
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // Çalışma kitabını kaydedin
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


