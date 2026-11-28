---
title: "Chart.GetActualSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart yöntemi. Grafiğin gerçek boyutunu piksel biriminde alır."
type: docs
url: /tr/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

Grafiğin gerçek boyutunu piksel biriminde alır.

```csharp
public int[] GetActualSize()
```

### Dönüş Değeri

Gerçek boyut bir dizi içinde (genişlik ve yükseklik). [0] genişlik; [1] yüksekliktir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
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
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);
            
            try
            {
                // GetActualSize yöntemini çağırın.
                int[] actualSize = chart.GetActualSize();
                
                // Sonucu göster
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // Grafik nesnesini yeniden boyutlandırarak etkiyi gösterin.
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


