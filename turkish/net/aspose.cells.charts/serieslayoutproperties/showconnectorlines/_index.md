---
title: "SeriesLayoutProperties.ShowConnectorLines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesLayoutProperties özelliği. Bağlantı hatlarının veri noktaları arasında gösterilip gösterilmediğini belirtir"
type: docs
url: /tr/net/aspose.cells.charts/serieslayoutproperties/showconnectorlines/
---
## SeriesLayoutProperties.ShowConnectorLines property

Veri noktaları arasında bağlayıcı çizgilerin gösterilip gösterilmediğini belirtir.

```csharp
public bool ShowConnectorLines { get; set; }
```

### Açıklamalar

Yalnızca Waterfall grafiği için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowConnectorLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];

            // ShowConnectorLines ve diğer özellikleri ayarla
            Aspose.Cells.Charts.SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowConnectorLines = true;
            layoutProperties.ShowMeanLine = true;

            workbook.Save("SeriesLayoutPropertiesShowConnectorLinesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


