---
title: "ChartArea.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartArea özelliği. Belirtilen ChartArea nesnesinin bir Font nesnesini alır"
type: docs
url: /tr/net/aspose.cells.charts/chartarea/font/
---
## ChartArea.Font property

`Font` nesnesini belirtilen ChartArea nesnesinden alır.

```csharp
public override Font Font { get; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(4000);
            worksheet.Cells["B5"].PutValue(6000);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Grafik alanını al
            ChartArea chartArea = chart.ChartArea;
            
            // Grafik alanı yazı tipi özelliklerini ayarla
            Aspose.Cells.Font font = chartArea.Font;
            font.Name = "Tahoma";
            font.Size = 10;
            font.Color = Color.Blue;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartAreaFontDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


