---
title: "ChartPoint.GetTopPointCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint yöntemi. Chart.Calculate yöntemi çağrıldıktan sonra üst noktaların sayısını alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/gettoppointcount/
---
## ChartPoint.GetTopPointCount method

Chart.Calculate() metodunu çağırdıktan sonra üst noktaların sayısını alır.

```csharp
public int GetTopPointCount()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointCountDemo
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
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Tüm özelliklerin ayarlandığından emin olmak için grafiği hesaplayın
            chart.Calculate();

            try
            {
                // İlk serideki ilk noktayı alın
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // GetTopPointCount metodunu çağır
                int topPointCount = point.GetTopPointCount();
                
                // Sonucu göster
                Console.WriteLine($"Number of top points: {topPointCount}");
                
                // Üst nokta koordinatlarını almayı göster
                if (topPointCount > 0)
                {
                    for (int i = 0; i < topPointCount; i++)
                    {
                        float x = point.GetTopPointXPx(i);
                        float y = point.GetTopPointYPx(i);
                        Console.WriteLine($"Top point {i + 1} coordinates: ({x}, {y})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointCount method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MethodGetTopPointCountDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


