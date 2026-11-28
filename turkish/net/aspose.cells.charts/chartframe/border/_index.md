---
title: "ChartFrame.Border"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Kenarı alır"
type: docs
url: /tr/net/aspose.cells.charts/chartframe/border/
---
## ChartFrame.Border property

Kenarı alır [`border`](../../../aspose.cells.drawing/line/).

```csharp
public virtual Line Border { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBorderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik başlığına eriş
            chart.Title.Text = "Chart Title with Custom Border";
            ChartFrame title = chart.Title;

            // Kenarlık özelliklerini yapılandır
            Line border = title.Border;
            border.Color = System.Drawing.Color.Red;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.Transparency = 0.3;
            border.DashType = MsoLineDashStyle.Solid;

            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


