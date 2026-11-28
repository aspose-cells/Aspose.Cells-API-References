---
title: "ChartArea.X"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartArea özelliği. Grafik alanının sol üst köşe sütunundan yatay offseti, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartarea/x/
---
## ChartArea.X property

Grafik alanının sol üst köşe sütunundan yatay offseti, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar.

```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine ChartArea.XRatioToChart özelliğini kullanın. X = XRatioToChart * 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Grafik alanını yapılandırın
            Aspose.Cells.Charts.ChartArea chartArea = chart.ChartArea;
            chartArea.X = 10; // Demonstrating X property usage
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;

            // Çıktıyı kaydet
            workbook.Save("ChartAreaXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


