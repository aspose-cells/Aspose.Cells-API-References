---
title: "PlotArea.WidthRatioToChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PlotArea özelliği. Çizim alanı sınırlama kutusunun genişliğini, grafik alanının oranı birimi cinsinden alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/plotarea/widthratiotochart/
---
## PlotArea.WidthRatioToChart property

Çizim alanı sınırlama kutusunun genişliğini, grafik alanının oranı biriminde alır veya ayarlar.

```csharp
public override double WidthRatioToChart { get; set; }
```

### Açıklamalar

Plot-area sınırlama kutusu, plot alanını, işaretçileri (işaretçi etiketlerini) ve işaretçilerin etrafındaki küçük bir kenarlığı içerir. Değer MS Excel tarafından oluşturulmadıysa, bu yöntemi çağırmadan önce lütfen Chart.Calculate() yöntemini çağırın.

Bu **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** ve **HeightRatioToChart** **PlotArea**'nin, plot-area sınırlama kutusunu temsil eder; bu kutu plot alanını, işaretçikleri (işaret etiketi) ve işaretçiklerin etrafındaki küçük bir kenarı içerir. Gerçek plot alanı boyutunu almak istiyorsanız, **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** ve **InnerHeightRatioToChart** özelliklerini çağırmalısınız.

Excel 2007 veya sonraki sürümler için, varsayılan değer sıfırdır. Değeri, Chart.Calculate() çağrıldıktan sonra almanız gerekir.

WidthPixel = WidthRatioToChart * chart.ChartObject.Width. Not: WidthRatioToChart ayarlandığında, IsInnerMode özelliği otomatik olarak false olarak ayarlanacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyWidthRatioToChartDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin ve onun plot alanını alın
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            PlotArea plotArea = chart.PlotArea;

            // Mevcut WidthRatioToChart değerini göster
            Console.WriteLine("Current WidthRatioToChart value: " + plotArea.WidthRatioToChart);

            // Genişlik oranını değiştirin ve etkiyi görün
            plotArea.WidthRatioToChart = 0.6; // 60% of chart width
            Console.WriteLine("WidthRatioToChart changed to: " + plotArea.WidthRatioToChart);

            // Çalışma kitabını kaydedin
            workbook.Save("PlotAreaWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


