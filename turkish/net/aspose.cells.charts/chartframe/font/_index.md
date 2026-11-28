---
title: "ChartFrame.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Belirtilen ChartFrame nesnesinin bir Font nesnesini alır"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/font/
---
## ChartFrame.Font property

Belirtilen ChartFrame nesnesinin bir `Font` nesnesini alır.

```csharp
public virtual Font Font { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyFontDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik başlığını ayarla ve font özelliklerini yapılandır
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            chart.Title.Font.Color = System.Drawing.Color.Blue;
            chart.Title.Font.CapsType = TextCapsType.None;
            chart.Title.Font.IsBold = true;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartFontDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


