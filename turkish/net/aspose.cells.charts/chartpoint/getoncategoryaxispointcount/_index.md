---
title: "ChartPoint.GetOnCategoryAxisPointCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint yöntemi. Chart.Calculate yöntemi çağrıldıktan sonra kategori eksenindeki nokta sayısını alır. Yalnızca alan grafiklerine uygulanır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/getoncategoryaxispointcount/
---
## ChartPoint.GetOnCategoryAxisPointCount method

Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki nokta sayısını alır. Yalnızca alan grafikleri için geçerlidir.

```csharp
public int GetOnCategoryAxisPointCount()
```

### Açıklamalar

2D alan grafiği 1, 3D alan grafiği 2 döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointCountDemo
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

            // Bir alan grafiği ekleyin.
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Tüm grafik noktalarının hesaplandığından emin olmak için grafiği hesaplayın.
            chart.Calculate();

            try
            {
                // İlk seriden ilk grafik noktasını al
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // GetOnCategoryAxisPointCount yöntemini çağırın.
                int pointCount = point.GetOnCategoryAxisPointCount();
                
                Console.WriteLine($"Number of points on category axis: {pointCount}");
                
                // Kategori eksenindeki her noktanın koordinatlarını gösterin.
                for (int i = 0; i < pointCount; i++)
                {
                    float x = point.GetOnCategoryAxisPointXPx(i);
                    float y = point.GetOnCategoryAxisPointYPx(i);
                    Console.WriteLine($"Point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointCount method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("MethodGetOnCategoryAxisPointCountDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


