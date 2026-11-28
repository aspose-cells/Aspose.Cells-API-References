---
title: "Enum MapChartRegionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.MapChartRegionType enum. Harita grafiğinin bölge tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/mapchartregiontype/
---
## MapChartRegionType enumeration

Harita grafiğinin bölge türünü temsil eder.

```csharp
public enum MapChartRegionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Otomatik |
| DataOnly | `1` | Yalnızca veri içerir. |
| CountryRegionList | `2` | Ülke bölge listesi. |
| World | `3` | Dünya. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartRegionTypeDemo
    {
        public static void MapChartRegionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Çalışma sayfasına bir harita grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Harita grafiğinin bölge tipini ayarla
            foreach (Series series in chart.NSeries)
            {
                series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MapChartRegionTypeExample.xlsx");

            // Sonucu çıktı olarak ver
            Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


