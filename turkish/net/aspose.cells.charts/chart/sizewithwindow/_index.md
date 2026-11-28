---
title: "Chart.SizeWithWindow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Microsoft Excel, grafiği grafik sayfası penceresinin boyutuna göre yeniden boyutlandırıyorsa doğru"
type: docs
url: /tr/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

Microsoft Excel, grafiği grafik sayfası penceresinin boyutuna göre yeniden boyutlandırıyorsa True.

```csharp
public bool SizeWithWindow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // SizeWithWindow özelliğini göster
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // SizeWithWindow özelliğini etkinleştir
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


