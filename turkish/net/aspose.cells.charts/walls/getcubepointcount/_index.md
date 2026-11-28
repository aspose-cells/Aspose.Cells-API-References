---
title: "Walls.GetCubePointCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Walls yöntemi. Chart.Calculate metodunu çağırdıktan sonra küp noktalarının sayısını alır"
type: docs
url: /tr/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

Chart.Calculate() metodunu çağırdıktan sonra küp noktalarının sayısını alır.

```csharp
public int GetCubePointCount()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // 3D bir grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Duvar özelliklerinin mevcut olmasını sağlamak için grafiği hesaplayın
            chart.Calculate();

            try
            {
                // Walls nesnesini alın
                Walls walls = chart.Walls;
                
                // GetCubePointCount metodunu çağırın
                int pointCount = walls.GetCubePointCount();
                
                // Sonucu göster
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // Çalışma kitabını kaydedin
                workbook.Save("WallsMethodGetCubePointCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointCount method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


