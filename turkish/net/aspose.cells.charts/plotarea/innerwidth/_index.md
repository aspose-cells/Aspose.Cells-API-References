---
title: "PlotArea.InnerWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PlotArea özelliği. Çizim alanının genişliğini, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells.charts/plotarea/innerwidth/
---
## PlotArea.InnerWidth property

Çizim alanının genişliğini, grafik alanının 1/4000 birimi cinsinden alır veya ayarlar.

```csharp
[Obsolete("Use PlotArea.InnerWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerWidth { get; set; }
```

### Açıklamalar

Plot-area sınırlama kutusu, plot alanını, işaretçileri (işaretçi etiketlerini) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() yöntemini çağırın.

Bu **X**, **Y**, **Width** ve **Height** **PlotArea**'nin, plot-area sınırlama kutusunu temsil eder; bu kutu plot alanını, işaretçikleri (işaret etiketi) ve işaretçiklerin etrafındaki küçük bir kenarı içerir. Gerçek plot alanı boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

Not: InnerWidth ayarlandığında, IsInnerMode özelliği otomatik olarak True olarak ayarlanacaktır.

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.InnerWidthRatioToChart özelliğini kullanın. InnerWidth = InnerWidthRatioToChart * 4000; Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyInnerWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafik verilerini ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Plot alanını yapılandır
            Aspose.Cells.Charts.PlotArea plotArea = chart.PlotArea;
            plotArea.InnerWidth = 2800; // Main demonstration of InnerWidth property
            plotArea.InnerHeight = 1800;
            plotArea.IsInnerMode = true;

            workbook.Save("PlotAreaInnerWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


