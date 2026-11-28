---
title: "Trendline.IsNameAuto"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür"
type: docs
url: /tr/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür.

```csharp
public bool IsNameAuto { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyIsNameAutoDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe seri ekle
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Trend çizgisi ekle - doğru Trendline nesnesi oluşturulmasını sağlamak için değiştirildi
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // IsNameAuto özelliğini göster
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // Özel ad ayarla (otomatik adlandırmayı devre dışı bırakır)
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // Otomatik ada sıfırla
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


