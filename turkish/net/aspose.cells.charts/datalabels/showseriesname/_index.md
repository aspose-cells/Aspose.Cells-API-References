---
title: "DataLabels.ShowSeriesName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Serinin adının bir grafikteki veri etiketlerinde gösterilip gösterilmeyeceğini belirtir. Serinin adını göstermek için true, gizlemek için false"
type: docs
url: /tr/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Seri adının bir grafikteki veri etiketlerinde gösterilip gösterilmeyeceğini belirtir. Doğru ise seri adı gösterilir. Yanlış ise gizlenir.

```csharp
public bool ShowSeriesName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // İlk seri için veri etiketlerini etkinleştir
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Belirli noktanın veri etiketi için seri adının gösterilmesini etkinleştir
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // Grafiği hesapla
            chart.Calculate();

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


