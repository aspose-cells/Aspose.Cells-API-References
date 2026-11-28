---
title: "PlotArea.Y"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PlotArea özelliği. Grafik alanının 1/4000 birimi cinsinden plotarea sınırlama kutusunun üst‑üst köşesinin y koordinatını alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells.charts/plotarea/y/
---
## PlotArea.Y property

Plot-area sınırlama kutusunun üst‑üst köşesinin y koordinatını, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar.

```csharp
[Obsolete("Use PlotArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Açıklamalar

Plot-area sınırlama kutusu, plot alanını, işaretçileri (işaretçi etiketlerini) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() yöntemini çağırın.

Bu **X**, **Y**, **Width** ve **Height** **PlotArea**'nin, plot-area sınırlama kutusunu temsil eder; bu kutu plot alanını, işaretçikleri (işaret etiketi) ve işaretçiklerin etrafındaki küçük bir kenarı içerir. Gerçek plot alanı boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

Not: Y ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanır.

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.YRatioToChart özelliğini kullanın. Y = YRatioToChart * 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(50);

            // Grafik oluştur
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Grafik verilerini ayarla
            chart.NSeries.Add("B1:B2", false);
            chart.NSeries.CategoryData = "A1:A2";

            // Plot alanını yapılandır
            chart.PlotArea.Width = 300;
            chart.PlotArea.Height = 200;
            chart.PlotArea.X = 100;
            chart.PlotArea.Y = 150; // Demonstrating Y property usage

            // Çalışma kitabını kaydedin
            workbook.Save("PlotAreaPropertyYDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


