---
title: "Axis.TickLabelPosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Belirtilen eksende tik işareti etiketlerinin konumunu temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axis/ticklabelposition/
---
## Axis.TickLabelPosition property

Belirtilen eksende işaretleme etiketi konumunu temsil eder.

```csharp
public TickLabelPositionType TickLabelPosition { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelPositionDemo
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
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Tik etiketi konumunu ayarla
            chart.CategoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            
            // Çalışma kitabını kaydedin
            workbook.Save("AxisPropertyTickLabelPositionDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TickLabelPositionType](../../ticklabelpositiontype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


