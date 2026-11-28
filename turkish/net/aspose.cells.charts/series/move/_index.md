---
title: "Series.Move"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series yöntemi. Seriyi yukarı veya aşağı hareket ettirir"
type: docs
url: /tr/net/aspose.cells.charts/series/move/
---
## Series.Move method

Seriyi yukarı veya aşağı hareket ettirir.

```csharp
public void Move(int count)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayım | Int32 | Yukarı veya aşağı hareket sayısı. Bu sıfırdan küçükse seriyi yukarı taşı; bu sıfırdan büyükse seriyi aşağı taşı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
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
            
            // Grafiğe seri ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // İlk seriyi al
            Series series = chart.NSeries[0];
            
            try
            {
                // Int32 parametresiyle Move metodunu çağırın
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // Seri adını değiştirerek etkiyi gösterin
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


