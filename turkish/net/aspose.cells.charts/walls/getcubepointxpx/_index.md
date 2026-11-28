---
title: "Walls.GetCubePointXPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Walls yöntemi. Chart.Calculate yöntemini çağırdıktan sonra, walls küpünün tepe noktasının x koordinatını alır. Walls küpünün tepe noktası sayısı sekizdir."
type: docs
url: /tr/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

Chart.Calculate() metodunu çağırdıktan sonra duvar küpünün tepe noktasının x koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir

```csharp
public float GetCubePointXPx(int index)
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointXPxWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // 3D bir grafik oluşturun
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Duvar özelliklerinin mevcut olmasını sağlamak için grafiği hesaplayın
            chart.Calculate();

            // Walls nesnesini alın
            Walls walls = chart.Walls;

            try
            {
                // Küp nokta sayısını alın
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // GetCubePointXPx yöntemini indeks 0 (ilk nokta) ile çağırın
                    float xCoordinate = walls.GetCubePointXPx(0);
                    
                    Console.WriteLine($"X coordinate of first cube point in pixels: {xCoordinate}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointXPx method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


