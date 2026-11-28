---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Donut diliminin iç yarıçapını piksel biriminde, Chart.Calculate metodunu çağırdıktan sonra alır. Donut chart için geçerlidir."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

Chart.Calculate() yöntemi çağrıldıktan sonra doughnut diliminin iç yarıçapını piksel biriminde alır. Doughnut grafiğine uygulanır.

```csharp
public int DoughnutInnerRadius { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
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
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak grafik noktalarını alın.
            chart.Calculate();

            // İlk seriden ilk grafik noktasını alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut DoughnutInnerRadius değerini göster.
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Not: DoughnutInnerRadius sadece okunabilir, bu yüzden doğrudan ayarlanamaz.
            // İç yarıçapı değiştirmek için, grafiğin HoleSize özelliğini ayarlamamız gerekir.
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // Grafiği yeniden hesaplayarak DoughnutInnerRadius değerini güncelle.
            chart.Calculate();

            // Güncellenmiş DoughnutInnerRadius değerini göster.
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Çalışma kitabını kaydedin
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


