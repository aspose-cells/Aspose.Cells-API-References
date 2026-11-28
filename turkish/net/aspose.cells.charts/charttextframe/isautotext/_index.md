---
title: "ChartTextFrame.IsAutoText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartTextFrame özelliği. Metnin otomatik olarak oluşturulduğunu gösterir"
type: docs
url: /tr/net/aspose.cells.charts/charttextframe/isautotext/
---
## ChartTextFrame.IsAutoText property

Metnin otomatik oluşturulduğunu gösterir.

```csharp
public virtual bool IsAutoText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsAutoTextDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafik verilerini ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik başlığını yapılandır
            Aspose.Cells.Charts.ChartTextFrame title = chart.Title;
            title.Text = "Custom Chart Title";
            
            // IsAutoText özelliğini göster
            title.IsAutoText = false; // Disable auto-generated text
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartTextFrame_IsAutoText_Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


