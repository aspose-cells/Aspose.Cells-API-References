---
title: "ChartPoint.GetBottomPointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint yöntemi. Chart.Calculate yöntemi çağrıldıktan sonra şeklin alt noktasının y koordinatını alır. 3B grafikler Column3D, Bar3D, Cone, Cylinder, Pyramid için geçerlidir"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/getbottompointypx/
---
## ChartPoint.GetBottomPointYPx method

Chart.Calculate() metodunu çağırdıktan sonra şeklin alt noktasının y koordinatını alır. 3D grafikler için geçerlidir: Column3D, Bar3D, Cone, Cylinder, Pyramid

```csharp
public float GetBottomPointYPx(int index)
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointYPxDemo
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
            
            // Seri ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Grafiği hesapla, tüm noktaların hesaplandığından emin olmak için
            chart.Calculate();
            
            // İlk serinin ilk noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Alt noktaların sayısını al
                int bottomPointCount = point.GetBottomPointCount();
                
                if (bottomPointCount > 0)
                {
                    // GetBottomPointYPx yöntemini dizin 0 ile çağır
                    float yPx = point.GetBottomPointYPx(0);
                    
                    Console.WriteLine($"Bottom point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointYPx method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MethodGetBottomPointYPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


