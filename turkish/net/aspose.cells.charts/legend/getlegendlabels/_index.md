---
title: "Legend.GetLegendLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Legend yöntemi. Chart.Calculate yöntemi çağrıldıktan sonra lejant girişlerinin etiketlerini alır"
type: docs
url: /tr/net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

Chart.Calculate() yöntemi çağrıldıktan sonra başlık girişlerinin etiketlerini alır.

```csharp
public string[] GetLegendLabels()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendMethodGetLegendLabelsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Grafiği hesapla
            chart.Calculate();
            
            // Lejant etiketlerini al
            string[] legendLabels = chart.Legend.GetLegendLabels();
            
            // Lejant etiketlerini göster
            Console.WriteLine("Legend Labels:");
            foreach (string label in legendLabels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


