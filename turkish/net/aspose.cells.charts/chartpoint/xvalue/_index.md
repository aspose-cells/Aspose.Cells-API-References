---
title: "ChartPoint.XValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Grafik noktasının X değerini alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/xvalue/
---
## ChartPoint.XValue property

Grafik noktasının X değerini alır veya ayarlar.

```csharp
public object XValue { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyXValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleniyor
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(50);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Bir grafik ekleniyor
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri kaynağı ayarlanıyor
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Veri noktaları özelleştiriliyor
            for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
            {
                ChartPoint point = chart.NSeries[0].Points[i];
                
                // XValue özelliği kullanımını gösterme
                point.XValue = "Modified " + (i + 1);
                
                // Görünürlük için ek biçimlendirme
                point.Area.ForegroundColor = Color.FromArgb(100 + i * 50, 150, 200);
            }

            workbook.Save("ChartPointXValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


