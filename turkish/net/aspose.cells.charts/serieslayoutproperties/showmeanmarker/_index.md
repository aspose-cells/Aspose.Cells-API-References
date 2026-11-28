---
title: "SeriesLayoutProperties.ShowMeanMarker"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesLayoutProperties özelliği. Ortalamayı gösteren işaretçilerin gösterilip gösterilmediğini belirtir"
type: docs
url: /tr/net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

Ortalama gösteren işaretçilerin gösterilip gösterilmeyeceğini belirtir.

```csharp
public bool ShowMeanMarker { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Grafik oluştur (ortalama işaretçilerini destekleyen Sütun grafik türünü kullanarak)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Seri ekle
            chart.NSeries.Add("A1:A4", true);
            Series series = chart.NSeries[0];

            // ShowMeanMarker ile düzen özelliklerini yapılandır
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowMeanLine = true;

            // Çıktıyı kaydet
            workbook.Save("ColumnChartWithMeanMarker.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


