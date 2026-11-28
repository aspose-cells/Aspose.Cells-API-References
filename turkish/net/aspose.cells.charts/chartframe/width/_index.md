---
title: "ChartFrame.Width"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Çerçevenin genişliğini, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Çerçevenin genişliğini, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Açıklamalar

1/4000 birimini piksele nasıl dönüştürülür? Piksel Cinsinden Genişlik = Genişlik * Chart.ChartObject.Height / 4000d;

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartFrame.WidthRatioToChart özelliğini kullanın. Genişlik = WidthRatioToChart * 4000; Bu özellik Şubat 2025'ten itibaren 12 ay içinde kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyWidthDemo
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

            // Bir grafik ekleyin ve grafik çerçevesini alın
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            ChartFrame chartFrame = chart.ChartArea;

            // Orijinal genişliği ayarla ve göster
            chartFrame.Width = 800;
            Console.WriteLine("Original Width: " + chartFrame.Width);

            // Genişliği değiştir
            chartFrame.Width = 1000;
            Console.WriteLine("Modified Width: " + chartFrame.Width);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFrameWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


