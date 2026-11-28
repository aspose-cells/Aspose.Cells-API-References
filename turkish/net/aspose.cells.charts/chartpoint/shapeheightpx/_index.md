---
title: "ChartPoint.ShapeHeightPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra yüksekliği piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapeheightpx/
---
## ChartPoint.ShapeHeightPx property

Chart.Calculate() metodunu çağırdıktan sonra yüksekliği piksel biriminde alır.

```csharp
public int ShapeHeightPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightPxDemo
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

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Şekil boyutlarını elde etmek için grafiği hesaplayın
            chart.Calculate();

            // İlk seriden ilk grafik noktasını alın
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Grafik noktasının şeklinin mevcut yüksekliğini piksel olarak gösterin
            Console.WriteLine("Current ShapeHeightPx value: " + chartPoint.ShapeHeightPx);

            // Not: ShapeHeightPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamıyoruz
            // Yüksekliği değiştirmek için grafik boyutunu veya veri değerlerini değiştirmeniz gerekir
            // ve grafiği yeniden hesaplayın

            // Grafik noktasının boyutunu etkileyecek veri değerini değiştirin
            worksheet.Cells["B2"].PutValue(50);
            chart.Calculate();

            // Veriyi değiştirdikten sonra yeni yüksekliği gösterin
            Console.WriteLine("New ShapeHeightPx value after data change: " + chartPoint.ShapeHeightPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointShapeHeightPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


