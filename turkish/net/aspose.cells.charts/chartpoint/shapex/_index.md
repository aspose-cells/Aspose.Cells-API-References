---
title: "ChartPoint.ShapeX"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra grafiğin genişliğinin 1/4000 biriminde sol üst köşenin x koordinatını alır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapex/
---
## ChartPoint.ShapeX property

Chart.Calculate() metodunu çağırdıktan sonra grafiğin genişliğinin 1/4000 biriminde sol üst köşenin x koordinatını alır.

```csharp
public int ShapeX { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXDemo
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
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // ShapeX'in doldurulduğundan emin olmak için grafiği hesaplayın.
            chart.Calculate();

            // İlk serideki ilk noktayı alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // ShapeX değerini (grafiğin genişliğinin 1/4000'i) gösterin.
            Console.WriteLine("ShapeX value (1/4000 units): " + point.ShapeX);
            Console.WriteLine("ShapeX value (pixels): " + point.ShapeXPx);

            // ShapeX'i, öğeleri grafik noktasına göre konumlandırmak için kullanmayı gösterin.
            // Not: ShapeX yalnızca okunabilir olduğundan, doğrudan değiştiremiyoruz,
            // ancak diğer öğeleri konumlandırmak için kullanabiliriz.
            if (point.ShapeX > 0)
            {
                // Grafik noktasının X konumuna hizalanmış bir metin kutusu ekleyin.
                Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(
                    point.ShapeXPx, 100, 100, 50, 100, 50);
                textBox.Text = "Point 1";
            }

            // Sonucu kaydet
            workbook.Save("ChartPointShapeXDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


