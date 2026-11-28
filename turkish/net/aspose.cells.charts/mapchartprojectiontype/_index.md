---
title: "Enum MapChartProjectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.MapChartProjectionType enum. Harita grafiğinin projeksiyon türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/mapchartprojectiontype/
---
## MapChartProjectionType enumeration

Harita grafiğinin projeksiyon türünü temsil eder.

```csharp
public enum MapChartProjectionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Otomatik |
| Mercator | `1` | Mercator |
| Miller | `2` | Miller |
| Albers | `3` | Albers |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartProjectionTypeDemo
    {
        public static void MapChartProjectionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Harita grafiği için çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(80);
            worksheet.Cells["B4"].PutValue(60);

            // Çalışma sayfasına bir harita grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Harita grafiği için projeksiyon türünü ayarla
            chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Projeksiyon türünü çıktı olarak ver
            Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);

            // Çalışma kitabını kaydedin
            workbook.Save("MapChartProjectionTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


