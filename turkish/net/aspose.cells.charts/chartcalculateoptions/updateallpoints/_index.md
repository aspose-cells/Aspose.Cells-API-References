---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartCalculateOptions özelliği. Grafik hesaplaması sırasında tüm veri noktalarının güncellenip güncellenmeyeceği. Varsayılan False. Grafikteki her veri noktasının değerini almak istediğinizde bunu true olarak ayarlayın. Bu parametre True olarak ayarlanırsa, grafik hesaplandığında yeni veri noktaları oluşturulabilir. Bu, Excel dosyasının daha büyük olmasına neden olabilir."
type: docs
url: /tr/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Grafik hesaplaması yapılırken tüm veri noktalarının güncellenip güncellenmeyeceği. Varsayılan: False. Grafikteki her bir veri noktasının değerini özellikle almak istediğinizde, bunu true olarak ayarlayın. Bu parametre True olarak ayarlanırsa, grafik hesaplandığında yeni veri noktaları oluşturulabilir. Bu, Excel dosyasının daha büyük olmasına neden olabilir.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Veri etiketlerini etkinleştir
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // Grafiği UpdateAllPoints seçeneğiyle hesapla
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // Sonucu göstermek için bazı veri etiketi değerlerini çıktı olarak ver
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


