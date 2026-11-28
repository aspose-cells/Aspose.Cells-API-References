---
title: "Enum MapChartLabelLayout"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.MapChartLabelLayout enum. Harita grafik etiketlerinin düzenini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

Harita grafiği etiketlerinin düzenini temsil eder.

```csharp
public enum MapChartLabelLayout
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| BestFitOnly | `0` | Yalnızca en iyi uyum kullanılır. |
| ShowAll | `1` | Tüm etiketleri gösterir. |
| None | `2` | Etiket yok. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartLabelLayoutDemo
    {
        public static void MapChartLabelLayoutExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Harita grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Çalışma sayfasına bir harita grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik için veri aralığını ayarlayın
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Seri düzen özelliklerine erişin
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Harita grafik etiketi düzenini ayarla
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // Çalışma kitabını kaydedin
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


