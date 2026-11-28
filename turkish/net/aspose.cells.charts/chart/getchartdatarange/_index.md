---
title: "Chart.GetChartDataRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart yöntemi. Grafiğin veri kaynağı aralığını alır"
type: docs
url: /tr/net/aspose.cells.charts/chart/getchartdatarange/
---
## Chart.GetChartDataRange method

Grafiğin veri kaynağı aralığını alır.

```csharp
public string GetChartDataRange()
```

### Dönüş Değeri

Veri kaynağı.

### Açıklamalar

Yalnızca aralığı destekler. Series.Values, Name ve XValues sürekli bir aralıkta ise, bunları içeren bir aralık döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodGetChartDataRangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C4"].PutValue(60);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("=Sheet1!$B$1:$C$4", true);
            
            // Grafik veri aralığını al ve göster
            string dataRange = chart.GetChartDataRange();
            Console.WriteLine("Chart Data Range: " + dataRange);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


