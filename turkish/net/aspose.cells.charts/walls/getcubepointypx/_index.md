---
title: "Walls.GetCubePointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Walls yöntemi. Chart.Calculate metodunu çağırdıktan sonra duvar küpünün tepe noktasının y koordinatını alır. Duvar küpünün tepe noktalarının sayısı sekizdir."
type: docs
url: /tr/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

Chart.Calculate() metodunu çağırdıktan sonra duvar küpünün tepe noktasının y koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir.

```csharp
public float GetCubePointYPx(int index)
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointYPxDemo
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

            // 3D bir grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Duvar özelliklerinin doldurulmasını sağlamak için grafiği hesaplayın
            chart.Calculate();

            // Walls nesnesini alın
            Walls walls = chart.Walls;

            try
            {
                // Küp noktalarının sayısını alın
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // GetCubePointYPx'i ilk indeksle (0) çağırın
                    float yPx = walls.GetCubePointYPx(0);
                    Console.WriteLine($"Y-coordinate of first cube point in pixels: {yPx}");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointYPx method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


