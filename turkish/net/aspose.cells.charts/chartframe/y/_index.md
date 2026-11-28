---
title: "ChartFrame.Y"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Üst sol köşenin y koordinatını, grafik alanının 1/4000 birimi olarak alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

Sol üst köşenin y koordinatını grafik alanının 1/4000 biriminde alır veya ayarlar.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### Açıklamalar

1/4000 birimini piksellere nasıl dönüştürülür? Y Pikselde = Y * Chart.ChartObject.Height / 4000d;

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine ChartFrame.YRatioToChart özelliğini kullanın. Y = YRatioToChart * 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyYDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Grafik ekle
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Grafik başlığına erişin ve Y konumunu ayarlayın
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrate Y property usage

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFramePropertyYDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


