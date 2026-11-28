---
title: "ChartPoint.InnerRadiusPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra doughnut diliminin iç yarıçapını piksel biriminde alır. Doughnut grafiklerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

Chart.Calculate() yöntemi çağrıldıktan sonra doughnut diliminin iç yarıçapını piksel biriminde alır. Doughnut grafiklerine uygulanır.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ChartPoint.DoughnutInnerRadius özelliğini kullanın. Bu özellik, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Bir doughnut grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik nokta özelliklerini elde etmek için grafiği hesaplayın
            chart.Calculate();

            // İlk seriden ilk grafik noktasını alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut iç yarıçap değerini göster (yalnızca okunabilir özellik)
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // Not: InnerRadiusPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // İç yarıçapı değiştirmek için doughnut deliği boyutunu ayarlamamız gerekir
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Özellikleri güncellemek için grafiği yeniden hesaplayın
            chart.Calculate();

            // Doughnut deliği boyutu değiştirildikten sonra yeni iç yarıçap değerini göster
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // Sonucu kaydet
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


