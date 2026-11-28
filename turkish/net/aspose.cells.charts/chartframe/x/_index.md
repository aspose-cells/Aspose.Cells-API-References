---
title: "ChartFrame.X"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Grafik alanının 1/4000 birimi cinsinden sol üst köşenin x koordinatını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Sol üst köşenin x koordinatını grafik alanının 1/4000 birimi cinsinden alır veya ayarlar.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Açıklamalar

1/4000 birimini piksellere nasıl dönüştürülür? X Pikselde = X * Chart.ChartObject.Width / 4000d;

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine ChartFrame.XRatioToChart özelliğini kullanın. X = XRatioToChart * 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyXDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Grafik ekle
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Seri ekleyin ve X/Y değerlerini ayarlayın
            chart.NSeries.Add("Sheet1!B2:B10", true);
            chart.NSeries[0].XValues = "Sheet1!A2:A10";

            // Trend çizgisi ekleyin
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            
            // Veri etiketlerini yapılandırın
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Blue;
            
            // X özelliğinin kullanımını gösterin
            trendline.DataLabels.X = -500; // Set X position offset
            trendline.DataLabels.Y = 200;  // Set Y position offset

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFramePropertyXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


