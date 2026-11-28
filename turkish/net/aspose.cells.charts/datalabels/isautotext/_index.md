---
title: "DataLabels.IsAutoText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Metnin otomatik olarak oluşturulduğunu gösterir"
type: docs
url: /tr/net/aspose.cells.charts/datalabels/isautotext/
---
## DataLabels.IsAutoText property

Metnin otomatik oluşturulduğunu gösterir.

```csharp
public override bool IsAutoText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsAutoTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
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

            // Veri etiketlerini etkinleştir
            foreach (Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
                
                // IsAutoText özelliğini göster
                foreach (ChartPoint point in series.Points)
                {
                    Console.WriteLine("IsAutoText before setting: " + point.DataLabels.IsAutoText);
                    point.DataLabels.IsAutoText = false;
                    point.DataLabels.Text = "Custom " + point.YValue;
                    Console.WriteLine("IsAutoText after setting: " + point.DataLabels.IsAutoText);
                    Console.WriteLine("DataLabel Text: " + point.DataLabels.Text);
                }
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsIsAutoTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


