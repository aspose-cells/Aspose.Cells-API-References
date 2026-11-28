---
title: "Sınıf SeriesLayoutProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.SeriesLayoutProperties sınıfı. Seri düzeninin özelliklerini temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/serieslayoutproperties/
---
## SeriesLayoutProperties class

Seri düzeninin özelliklerini temsil eder.

```csharp
public class SeriesLayoutProperties
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | Aralığın sol tarafta kapalı olup olmadığını gösterir. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | Haritanın projeksiyon tipini alır ve ayarlar. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | Haritanın bölge tipini alır ve ayarlar. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | Harita etiketlerinin düzenini alır ve ayarlar. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | Seri için istatistiksel özellikleri temsil eder. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | Veri noktaları arasında bağlayıcı çizgilerin gösterilip gösterilmediğini belirtir. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | Aykırı olmayan veri noktalarının gösterilip gösterilmeyeceğini belirtir. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | Tüm ortalama noktalarını birleştiren çizginin gösterilip gösterilmeyeceğini belirtir. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | Ortalama gösteren işaretçilerin gösterilip gösterilmeyeceğini belirtir. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | Uç değer veri noktalarının gösterilip gösterilmeyeceğini belirtir. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | Bir alt toplam veri noktasının dizinini temsil eder. |

### Açıklamalar

Yalnızca BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall ve Histogram grafiklerine uygulanabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesLayoutPropertiesDemo
    {
        public static void SeriesLayoutPropertiesExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe seri ekle
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];

            // Serinin değerlerini ayarla
            series.Values = "=B1:B4";

            // SeriesLayoutProperties nesnesine eriş
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;

            // SeriesLayoutProperties özelliklerini ayarla
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.QuartileCalculation = QuartileCalculationType.Inclusive;
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            layoutProperties.IsIntervalLeftClosed = true;
            layoutProperties.MapChartRegionType = MapChartRegionType.World;
            layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesLayoutPropertiesExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


