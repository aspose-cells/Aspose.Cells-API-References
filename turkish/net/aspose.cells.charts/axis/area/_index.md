---
title: "Axis.Area"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Area değerini alır"
type: docs
url: /tr/net/aspose.cells.charts/axis/area/
---
## Axis.Area property

`Area` değerini alır.

```csharp
public Area Area { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAreaDemo
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
            
            // Kategori eksen alanı özelliklerine erişin
            chart.CategoryAxis.Area.BackgroundColor = Color.LightBlue;
            chart.CategoryAxis.Area.ForegroundColor = Color.White;
            chart.CategoryAxis.Area.Formatting = FormattingType.Custom;
            
            // Çalışma kitabını kaydedin
            workbook.Save("AxisPropertyAreaDemo_Output.xlsx");
            
            Console.WriteLine("Category Axis Area Background Color: " + chart.CategoryAxis.Area.BackgroundColor);
        }
    }
}
```

### Ayrıca Bakınız

* class [Area](../../../aspose.cells.drawing/area/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


