---
title: "ChartPoint.GetTopPointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint yöntemi. Chart.Calculate yöntemi çağrıldıktan sonra şeklin üst noktasının y koordinatını alır. 3D grafikler Column3D, Bar3D, Cone, Cylinder, Pyramid ve Area3D için geçerlidir"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/gettoppointypx/
---
## ChartPoint.GetTopPointYPx method

Chart.Calculate() metodunu çağırdıktan sonra şeklin üst noktasının y-koordinatını alır. 3D grafiklere uygulanır: Column3D, Bar3D, Cone, Cylinder, Pyramid ve Area3D.

```csharp
public float GetTopPointYPx(int index)
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointYPxWithInt32Demo
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
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Tüm konum özelliklerinin hesaplandığından emin olmak için grafiği hesaplayın
            chart.Calculate();
            
            // İlk seriden ilk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Üst noktaların sayısını alın
                int topPointCount = point.GetTopPointCount();
                
                if (topPointCount > 0)
                {
                    // GetTopPointYPx'i indeks 0 ile çağırın
                    float yPx = point.GetTopPointYPx(0);
                    
                    Console.WriteLine($"Top point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointYPx method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ChartPointMethodGetTopPointYPxWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


