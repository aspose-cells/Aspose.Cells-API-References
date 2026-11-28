---
title: "DataLabels.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Veri etiketinin metnini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

Veri etiketinin metnini alır veya ayarlar.

```csharp
public override string Text { get; set; }
```

### Açıklamalar

Yalnızca bu bir grafik noktasının veri etiketi olduğunda çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["A4"].PutValue("Product C");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Veri etiketlerini etkinleştir
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Aspose.Cells.Charts.Series series = chart.NSeries[i];
                series.DataLabels.ShowValue = true;
                
                // Veri etiketi metnini özelleştir
                for (int j = 0; j < series.Points.Count; j++)
                {
                    series.Points[j].DataLabels.Text = $"+{series.Points[j].YValue}";
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


