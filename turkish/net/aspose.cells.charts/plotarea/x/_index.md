---
title: "PlotArea.X"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PlotArea özelliği. Grafik alanının 1/4000 biriminde, plotarea sınırlama kutusunun üst sol köşesinin x koordinatını alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells.charts/plotarea/x/
---
## PlotArea.X property

Plot-area sınırlama kutusunun üst sol köşesinin x koordinatını, grafik alanının 1/4000 biriminde alır veya ayarlar.

```csharp
[Obsolete("Use PlotArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Açıklamalar

Plot-area sınırlama kutusu, plot alanını, işaretçileri (işaretçi etiketlerini) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() yöntemini çağırın.

Bu **X**, **Y**, **Width** ve **Height** **PlotArea**'nin, plot-area sınırlama kutusunu temsil eder; bu kutu plot alanını, işaretçikleri (işaret etiketi) ve işaretçiklerin etrafındaki küçük bir kenarı içerir. Gerçek plot alanı boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

Not: X ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanır.

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine PlotArea.XRatioToChart özelliğini kullanın. X = XRatioToChart * 4000. Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyXDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
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

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // PlotArea özelliklerini ayarla
            chart.PlotArea.X = 100;  // Demonstrate X property usage
            chart.PlotArea.Y = 200;
            chart.PlotArea.Width = 1000;
            chart.PlotArea.Height = 800;

            // Çalışma kitabını kaydedin
            workbook.Save("PlotAreaPropertyXDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


