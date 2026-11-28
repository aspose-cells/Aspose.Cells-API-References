---
title: "ChartFrame.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Çerçevenin yüksekliğini, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Çerçevenin yüksekliğini, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Açıklamalar

1/4000 birimlerini piksele nasıl dönüştürülür? Piksel cinsinden Yükseklik = Y * Chart.ChartObject.Height / 4000d;

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartFrame.HeightRatioToChart özelliğini kullanın. Yükseklik = HeightRatioToChart * 4000. Bu özellik Şubat 2025 tarihinden itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Veri etiketlerine eriş
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Height özelliğini ayarla
            dataLabels.Height = 200; // Set height to 200 pixels
            
            // Yükseklik değerini göster
            Console.WriteLine("DataLabels Height: " + dataLabels.Height);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartFramePropertyHeightDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


