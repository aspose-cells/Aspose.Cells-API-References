---
title: "ChartPoint.GetBottomPointXPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint metodu. `Chart.Calculate` metodunu çağırdıktan sonra şeklin alt noktasının x koordinatını alır. 3D grafikler Column3D, Bar3D, Cone, Cylinder, Pyramid için geçerlidir"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/getbottompointxpx/
---
## ChartPoint.GetBottomPointXPx method

Chart.Calculate() metodunu çağırdıktan sonra şeklin alt noktasının x koordinatını alır. 3D grafikler için geçerlidir: Column3D, Bar3D, Cone, Cylinder, Pyramid

```csharp
public float GetBottomPointXPx(int index)
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointXPxWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
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

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Tüm konum özelliklerinin ayarlandığından emin olmak için grafiği hesapla
            chart.Calculate();

            try
            {
                // İlk seriden ilk grafik noktasını al
                ChartPoint point = chart.NSeries[0].Points[0];

                // Alt noktaların sayısını al
                int bottomPointCount = point.GetBottomPointCount();

                if (bottomPointCount > 0)
                {
                    // GetBottomPointXPx'i indeks 0 ile çağır
                    float xPos = point.GetBottomPointXPx(0);
                    Console.WriteLine($"X position of bottom point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointXPx method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("ChartPointMethodGetBottomPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


