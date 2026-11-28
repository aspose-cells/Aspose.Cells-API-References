---
title: "DataLabels.ShowCellRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Hücre aralığını veri etiketi olarak gösterip göstermeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Hücre aralığının veri etiketi olarak gösterilip gösterilmeyeceğini belirtir.

```csharp
public bool ShowCellRange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCellRangeDemo
    {
        public static void Run()
        {
            // Çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veriyi ayarla
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // ShowCellRange ile veri etiketlerini yapılandır
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCellRange = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.Font.Color = Color.Blue;

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsShowCellRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


