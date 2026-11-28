---
title: "Axis.Title"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Bu eksenin grafikteki başlığını alır"
type: docs
url: /tr/net/aspose.cells.charts/axis/title/
---
## Axis.Title property

Grafikteki bu eksenin başlığını alır.

```csharp
public Title Title { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTitleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Başlıkları yapılandır
            chart.Title.Text = "Sample Chart";
            chart.Title.IsVisible = true;
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            
            // Eksen başlıklarını yapılandır
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.IsVisible = true;
            chart.CategoryAxis.Title.Font.Name = "Arial";
            
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.IsVisible = true;
            chart.ValueAxis.Title.Font.Name = "Arial";
            
            // Çalışma kitabını kaydedin
            workbook.Save("AxisPropertyTitleDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


